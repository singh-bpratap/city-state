# city-state ruby gem

**city-state** is a very simple ruby gem to get a list of states in a country. Also, you can get a list of cities in a state, and a list of all countries of the world.

## Put this gem at your Gemfile:
```ruby
gem 'city-state', git: "https://github.com/singh-bpratap/city-state"
```

## List of states:
```ruby
CS.states(:us)
# => {:AK=>"Alaska", :AL=>"Alabama", :AR=>"Arkansas", :AZ=>"Arizona", :CA=>"California", :CO=>"Colorado", :CT=>"Connecticut", :DC=>"District of Columbia", :DE=>"Delaware", :FL=>"Florida", :GA=>"Georgia", :HI=>"Hawaii", :IA=>"Iowa", :ID=>"Idaho", :IL=>"Illinois", :IN=>"Indiana", :KS=>"Kansas", :KY=>"Kentucky", :LA=>"Louisiana", :MA=>"Massachusetts", :MD=>"Maryland", :ME=>"Maine", :MI=>"Michigan", :MN=>"Minnesota", :MO=>"Missouri", :MS=>"Mississippi", :MT=>"Montana", :NC=>"North Carolina", :ND=>"North Dakota", :NE=>"Nebraska", :NH=>"New Hampshire", :NJ=>"New Jersey", :NM=>"New Mexico", :NV=>"Nevada", :NY=>"New York", :OH=>"Ohio", :OK=>"Oklahoma", :OR=>"Oregon", :PA=>"Pennsylvania", :RI=>"Rhode Island", :SC=>"South Carolina", :SD=>"South Dakota", :TN=>"Tennessee", :TX=>"Texas", :UT=>"Utah", :VA=>"Virginia", :VT=>"Vermont", :WA=>"Washington", :WI=>"Wisconsin", :WV=>"West Virginia", :WY=>"Wyoming"} 
```

```ruby
CSForSelect.states(:IN)
# => [["Andaman and Nicobar", :AN], ["Andhra Pradesh", :AP], ["Arunachal Pradesh", :AR], ["Assam", :AS], ["Bihar", :BR], ["Chandigarh", :CH], ["Chhattisgarh", :CT], ["Dadra and Nagar Haveli", :DN], ["Daman and Diu", :DD], ["Goa", :GA], ["Gujarat", :GJ], ["Haryana", :HR], ["Himachal Pradesh", :HP], ["Jammu and Kashmir", :JK], ["Jharkhand", :JH], ["Karnataka", :KA], ["Kerala", :KL], ["Lakshadweep", :LD], ["Madhya Pradesh", :MP], ["Maharashtra", :MH], ["Manipur", :MN], ["Meghalaya", :ML], ["Mizoram", :MZ], ["Nagaland", :NL], ["National Capital Territory of Delhi", :DL], ["Odisha", :OR], ["Punjab", :PB], ["Rajasthan", :RJ], ["Sikkim", :SK], ["Tamil Nadu", :TN], ["Telangana", :TG], ["Tripura", :TR], ["Union Territory of Puducherry", :PY], ["Uttar Pradesh", :UP], ["Uttarakhand", :UT], ["West Bengal", :WB]]
```

**PS:** *city-state is case insensitive. You can use :US, :us, :Us, "us", "US", ...*

## List of cities:
```ruby
CS.cities(:ak, :us) / CSForSelect.cities(:ak, :us)
# => ["Adak", "Akhiok", "Akiachak", "Akiak", "Akutan", "Alakanuk", "Ambler", "Anchor Point", "Anchorage", "Angoon", "Atqasuk", "Barrow", "Bell Island Hot Springs", "Bethel", "Big Lake", "Buckland", "Chefornak", "Chevak", "Chicken", "Chugiak", "Coffman Cove", "Cooper Landing", "Copper Center", "Cordova", "Craig", "Deltana", "Dillingham", "Douglas", "Dutch Harbor", "Eagle River", "Eielson Air Force Base", "Fairbanks", "Fairbanks North Star Borough", "Fort Greely", "Fort Richardson", "Galena", "Girdwood", "Goodnews Bay", "Haines", "Homer", "Hooper Bay", "Juneau", "Kake", "Kaktovik", "Kalskag", "Kenai", "Ketchikan", "Kiana", "King Cove", "King Salmon", "Kipnuk", "Klawock", "Kodiak", "Kongiganak", "Kotlik", "Koyuk", "Kwethluk", "Levelock", "Manokotak", "May Creek", "Mekoryuk", "Metlakatla", "Mountain Village", "Nabesna", "Naknek", "Nazan Village", "Nenana", "New Stuyahok", "Nikiski", "Ninilchik", "Noatak", "Nome", "Nondalton", "Noorvik", "North Pole", "Northway", "Old Kotzebue", "Palmer", "Pedro Bay", "Petersburg", "Pilot Station", "Point Hope", "Point Lay", "Prudhoe Bay", "Russian Mission", "Sand Point", "Scammon Bay", "Selawik", "Seward", "Shungnak", "Sitka", "Skaguay", "Soldotna", "Stebbins", "Sterling", "Sutton", "Talkeetna", "Teller", "Thorne Bay", "Togiak", "Tok", "Toksook Bay", "Tuntutuliak", "Two Rivers", "Unalakleet", "Unalaska", "Valdez", "Wainwright", "Wasilla"]
```



## All countries of the world:
```ruby
CS.countries
# => {:AD=>"Andorra", :AE=>"United Arab Emirates", :AF=>"Afghanistan", :AG=>"Antigua and Barbuda", :AI=>"Anguilla", :AL=>"Albania", :AM=>"Armenia", :AO=>"Angola", :AQ=>"Antarctica", :AR=>"Argentina", :AS=>"American Samoa", :AT=>"Austria", :AU=>"Australia", :AW=>"Aruba", :AX=>"Åland", :AZ=>"Azerbaijan", :BA=>"Bosnia and Herzegovina", :BB=>"Barbados", :BD=>"Bangladesh", :BE=>"Belgium", :BF=>"Burkina Faso", :BG=>"Bulgaria", :BH=>"Bahrain", :BI=>"Burundi", :BJ=>"Benin", :BL=>"Saint-Barthélemy", :BM=>"Bermuda", :BN=>"Brunei", :BO=>"Bolivia", :BQ=>"Bonaire", :BR=>"Brazil", :BS=>"Bahamas", :BT=>"Bhutan", :BW=>"Botswana", :BY=>"Belarus", :BZ=>"Belize", :CA=>"Canada", :CC=>"Cocos [Keeling] Islands", :CD=>"Congo", :CF=>"Central African Republic", :CG=>"Republic of the Congo"}
```

```ruby
CSForSelect.countries
# => [["Afghanistan", :AF], ["Albania", :AL], ["Algeria", :DZ], ["American Samoa", :AS], ["Andorra", :AD], ["Angola", :AO], ["Anguilla", :AI], ["Antarctica", :AQ], ["Antigua and Barbuda", :AG], ["Argentina", :AR], ["Armenia", :AM], ["Aruba", :AW], ["Australia", :AU], ["Austria", :AT], ["Azerbaijan", :AZ], ["Bahamas", :BS], ["Bahrain", :BH], ["Bangladesh", :BD], ["Barbados", :BB], ["Belarus", :BY], ["Belgium", :BE], ["Belize", :BZ], ["Benin", :BJ], ["Bermuda", :BM], ["Bhutan", :BT], ["Bolivia", :BO], ["Bonaire", :BQ], ["Bosnia and Herzegovina", :BA], ["Botswana", :BW], ["Bouvet Island", :BV], ["Brazil", :BR], ["British Indian Ocean Territory", :IO], ["British Virgin Islands", :VG], ["Brunei", :BN], ["Bulgaria", :BG], ["Burkina Faso", :BF], ["Burundi", :BI], ["Cabo Verde", :CV], ["Cambodia", :KH], ["Cameroon", :CM], ["Canada", :CA], ["Cayman Islands", :KY], ["Central African Republic", :CF], ["Chad", :TD], ["Chile", :CL], ["China", :CN], ["Christmas Island", :CX], ["Cocos [Keeling] Islands", :CC], ["Colombia", :CO], ["Comoros", :KM], ["Congo", :CD], ["Cook Islands", :CK], ["Costa Rica", :CR], ["Croatia", :HR], ["Cuba", :CU], ["Curaçao", :CW], ["Cyprus", :CY], ["Czechia", :CZ], ["Democratic Republic of Timor-Leste", :TL], ["Denmark", :DK], ["Djibouti", :DJ], ["Dominica", :DM], ["Dominican Republic", :DO], ["Ecuador", :EC], ["Egypt", :EG], ["El Salvador", :SV], ["Equatorial Guinea", :GQ], ["Eritrea", :ER], ["Estonia", :EE], ["Eswatini", :SZ], ["Ethiopia", :ET], ["Falkland Islands", :FK], ["Faroe Islands", :FO], ["Federated States of Micronesia", :FM], ["Fiji", :FJ], ["Finland", :FI], ["France", :FR], ["French Guiana", :GF], ["French Polynesia", :PF], ["French Southern Territories", :TF], ["Gabon", :GA], ["Gambia", :GM], ["Georgia", :GE], ["Germany", :DE], ["Ghana", :GH], ["Gibraltar", :GI], ["Greece", :GR], ["Greenland", :GL], ["Grenada", :GD], ["Guadeloupe", :GP], ["Guam", :GU], ["Guatemala", :GT], ["Guernsey", :GG], ["Guinea", :GN], ["Guinea-Bissau", :GW], ["Guyana", :GY], ["Haiti", :HT], ["Hashemite Kingdom of Jordan", :JO], ["Heard Island and McDonald Islands", :HM], ["Honduras", :HN], ["Hong Kong", :HK], ["Hungary", :HU], ["Iceland", :IS], ["India", :IN], ["Indonesia", :ID], ["Iran", :IR], ["Iraq", :IQ], ["Ireland", :IE], ["Isle of Man", :IM], ["Israel", :IL], ["Italy", :IT], ["Ivory Coast", :CI], ["Jamaica", :JM], ["Japan", :JP], ["Jersey", :JE], ["Kazakhstan", :KZ], ["Kenya", :KE], ["Kiribati", :KI], ["Kosovo", :XK], ["Kuwait", :KW], ["Kyrgyzstan", :KG], ["Laos", :LA], ["Latvia", :LV], ["Lebanon", :LB], ["Lesotho", :LS], ["Liberia", :LR], ["Libya", :LY], ["Liechtenstein", :LI], ["Luxembourg", :LU], ["Macao", :MO], ["Macedonia", :MK], ["Madagascar", :MG], ["Malawi", :MW], ["Malaysia", :MY], ["Maldives", :MV], ["Mali", :ML], ["Malta", :MT], ["Marshall Islands", :MH], ["Martinique", :MQ], ["Mauritania", :MR], ["Mauritius", :MU], ["Mayotte", :YT], ["Mexico", :MX], ["Monaco", :MC], ["Mongolia", :MN], ["Montenegro", :ME], ["Montserrat", :MS], ["Morocco", :MA], ["Mozambique", :MZ], ["Myanmar", :MM], ["Namibia", :NA], ["Nauru", :NR], ["Nepal", :NP], ["Netherlands", :NL], ["New Caledonia", :NC], ["New Zealand", :NZ], ["Nicaragua", :NI], ["Niger", :NE], ["Nigeria", :NG], ["Niue", :NU], ["Norfolk Island", :NF], ["North Korea", :KP], ["Northern Mariana Islands", :MP], ["Norway", :NO], ["Oman", :OM], ["Pakistan", :PK], ["Palau", :PW], ["Palestine", :PS], ["Panama", :PA], ["Papua New Guinea", :PG], ["Paraguay", :PY], ["Peru", :PE], ["Philippines", :PH], ["Pitcairn Islands", :PN], ["Poland", :PL], ["Portugal", :PT], ["Puerto Rico", :PR], ["Qatar", :QA], ["Republic of Lithuania", :LT], ["Republic of Moldova", :MD], ["Republic of the Congo", :CG], ["Romania", :RO], ["Russia", :RU], ["Rwanda", :RW], ["Réunion", :RE], ["Saint Barthélemy", :BL], ["Saint Helena", :SH], ["Saint Lucia", :LC], ["Saint Martin", :MF], ["Saint Pierre and Miquelon", :PM], ["Saint Vincent and the Grenadines", :VC], ["Samoa", :WS], ["San Marino", :SM], ["Saudi Arabia", :SA], ["Senegal", :SN], ["Serbia", :RS], ["Seychelles", :SC], ["Sierra Leone", :SL], ["Singapore", :SG], ["Sint Maarten", :SX], ["Slovakia", :SK], ["Slovenia", :SI], ["Solomon Islands", :SB], ["Somalia", :SO], ["South Africa", :ZA], ["South Georgia and the South Sandwich Islands", :GS], ["South Korea", :KR], ["South Sudan", :SS], ["Spain", :ES], ["Sri Lanka", :LK], ["St Kitts and Nevis", :KN], ["Sudan", :SD], ["Suriname", :SR], ["Svalbard and Jan Mayen", :SJ], ["Sweden", :SE], ["Switzerland", :CH], ["Syria", :SY], ["São Tomé and Príncipe", :ST], ["Taiwan", :TW], ["Tajikistan", :TJ], ["Tanzania", :TZ], ["Thailand", :TH], ["Togo", :TG], ["Tokelau", :TK], ["Tonga", :TO], ["Trinidad and Tobago", :TT], ["Tunisia", :TN], ["Turkey", :TR], ["Turkmenistan", :TM], ["Turks and Caicos Islands", :TC], ["Tuvalu", :TV], ["U.S. Minor Outlying Islands", :UM], ["U.S. Virgin Islands", :VI], ["Uganda", :UG], ["Ukraine", :UA], ["United Arab Emirates", :AE], ["United Kingdom", :GB], ["United States", :US], ["Uruguay", :UY], ["Uzbekistan", :UZ], ["Vanuatu", :VU], ["Vatican City", :VA], ["Venezuela", :VE], ["Vietnam", :VN], ["Wallis and Futuna", :WF], ["Western Sahara", :EH], ["Yemen", :YE], ["Zambia", :ZM], ["Zimbabwe", :ZW], ["country_name", :COUNTRY_ISO_CODE], ["Åland", :AX]]
```

## Simplified syntax with *get* method:
* _CS.get_: list of countries (equivalent to `CS.countries`)
* _CS.get(country)_: list of states (equivalent to `CS.states(country)`)
* _CS.get(country, state)_: list of cities (equivalent to `CS.cities(state, country)`)

Example:
```ruby
CS.get
# => {:AD=>"Andorra", :AE=>"United Arab Emirates", :AF=>"Afghanistan", :AG=>"Antigua and Barbuda", :AI=>"Anguilla", :AL=>"Albania", :AM=>"Armenia", :AO=>"Angola", :AQ=>"Antarctica", :AR=>"Argentina", :AS=>"American Samoa", :AT=>"Austria", :AU=>"Australia", :AW=>"Aruba", :AX=>"Åland", :AZ=>"Azerbaijan", :BA=>"Bosnia and Herzegovina", :BB=>"Barbados", :BD=>"Bangladesh", :BE=>"Belgium", :BF=>"Burkina Faso", :BG=>"Bulgaria", :BH=>"Bahrain", :BI=>"Burundi", :BJ=>"Benin", :BL=>"Saint-Barthélemy", :BM=>"Bermuda", :BN=>"Brunei", :BO=>"Bolivia", :BQ=>"Bonaire", :BR=>"Brazil", :BS=>"Bahamas", :BT=>"Bhutan", :BW=>"Botswana", :BY=>"Belarus", :BZ=>"Belize", :CA=>"Canada", :CC=>"Cocos [Keeling] Islands", :CD=>"Congo", :CF=>"Central African Republic", :CG=>"Republic of the Congo"}
```
```ruby
CS.get :us
# => {:AK=>"Alaska", :AL=>"Alabama", :AR=>"Arkansas", :AZ=>"Arizona", :CA=>"California", :CO=>"Colorado", :CT=>"Connecticut", :DC=>"District of Columbia", :DE=>"Delaware", :FL=>"Florida", :GA=>"Georgia", :HI=>"Hawaii", :IA=>"Iowa", :ID=>"Idaho", :IL=>"Illinois", :IN=>"Indiana", :KS=>"Kansas", :KY=>"Kentucky", :LA=>"Louisiana", :MA=>"Massachusetts", :MD=>"Maryland", :ME=>"Maine", :MI=>"Michigan", :MN=>"Minnesota", :MO=>"Missouri", :MS=>"Mississippi", :MT=>"Montana", :NC=>"North Carolina", :ND=>"North Dakota", :NE=>"Nebraska", :NH=>"New Hampshire", :NJ=>"New Jersey", :NM=>"New Mexico", :NV=>"Nevada", :NY=>"New York", :OH=>"Ohio", :OK=>"Oklahoma", :OR=>"Oregon", :PA=>"Pennsylvania", :RI=>"Rhode Island", :SC=>"South Carolina", :SD=>"South Dakota", :TN=>"Tennessee", :TX=>"Texas", :UT=>"Utah", :VA=>"Virginia", :VT=>"Vermont", :WA=>"Washington", :WI=>"Wisconsin", :WV=>"West Virginia", :WY=>"Wyoming"} 
```
```ruby
CS.get :us, :ak
# => ["Adak", "Akhiok", "Akiachak", "Akiak", "Akutan", "Alakanuk", "Ambler", "Anchor Point", "Anchorage", "Angoon", "Atqasuk", "Barrow", "Bell Island Hot Springs", "Bethel", "Big Lake", "Buckland", "Chefornak", "Chevak", "Chicken", "Chugiak", "Coffman Cove", "Cooper Landing", "Copper Center", "Cordova", "Craig", "Deltana", "Dillingham", "Douglas", "Dutch Harbor", "Eagle River", "Eielson Air Force Base", "Fairbanks", "Fairbanks North Star Borough", "Fort Greely", "Fort Richardson", "Galena", "Girdwood", "Goodnews Bay", "Haines", "Homer", "Hooper Bay", "Juneau", "Kake", "Kaktovik", "Kalskag", "Kenai", "Ketchikan", "Kiana", "King Cove", "King Salmon", "Kipnuk", "Klawock", "Kodiak", "Kongiganak", "Kotlik", "Koyuk", "Kwethluk", "Levelock", "Manokotak", "May Creek", "Mekoryuk", "Metlakatla", "Mountain Village", "Nabesna", "Naknek", "Nazan Village", "Nenana", "New Stuyahok", "Nikiski", "Ninilchik", "Noatak", "Nome", "Nondalton", "Noorvik", "North Pole", "Northway", "Old Kotzebue", "Palmer", "Pedro Bay", "Petersburg", "Pilot Station", "Point Hope", "Point Lay", "Prudhoe Bay", "Russian Mission", "Sand Point", "Scammon Bay", "Selawik", "Seward", "Shungnak", "Sitka", "Skaguay", "Soldotna", "Stebbins", "Sterling", "Sutton", "Talkeetna", "Teller", "Thorne Bay", "Togiak", "Tok", "Toksook Bay", "Tuntutuliak", "Two Rivers", "Unalakleet", "Unalaska", "Valdez", "Wainwright", "Wasilla"]
```

## Update the database from MaxMind:
MaxMind update their databases weekly on tuesdays. To get a new and updated version, you can update with:
```ruby
CS.update
```

## Another countries:

When getting a city list, you can also specifies the country:
```ruby
CS.cities(:sp, :br)
```

The country is an optional argument. **city-state** always uses the last country that you used.
```ruby
CS.states(:br)
# => {:AC=>"Acre", :AL=>"Alagoas", :AM=>"Amazonas", :AP=>"Amapa", :BA=>"Bahia", :CE=>"Ceara", :DF=>"Federal District", :ES=>"Espirito Santo", :GO=>"Goias", :MA=>"Maranhao", :MG=>"Minas Gerais", :MS=>"Mato Grosso do Sul", :MT=>"Mato Grosso", :PA=>"Para", :PB=>"Paraiba", :PE=>"Pernambuco", :PI=>"Piaui", :PR=>"Parana", :RJ=>"Rio de Janeiro", :RN=>"Rio Grande do Norte", :RO=>"Rondonia", :RR=>"Roraima", :RS=>"Rio Grande do Sul", :SC=>"Santa Catarina", :SE=>"Sergipe", :SP=>"Sao Paulo", :TO=>"Tocantins"}
CS.cities(:to)
# => ["Aparecida do Rio Negro", "Araguaína", "Brejinho de Nazare", "Gurupi", "Itaguatins", "Miracema do Tocantins", "Monte Alegre", "Palmas", "Paraiso do Tocantins", "Parana", "Pedro Afonso", "Porto Nacional", "Presidente Kennedy", "Salvador", "Santo Antonio", "Sao Domingos", "Taguatinga", "Tucum"] 
```

# More details about this gem
http://www.learnwithdaniel.com/2015/02/citystate-list-of-cities-and-states-ruby/

# CityState License
**city-state** is a open source project by Daniel Loureiro with a MIT license. Also, it uses MaxMind open source database.

# MaxMind License
Database and Contents Copyright (c) 2015 MaxMind, Inc.
This work is licensed under the Creative Commons Attribution 3.0 Unported License. To view a copy of this license, visit http://creativecommons.org/licenses/by/3.0/.
