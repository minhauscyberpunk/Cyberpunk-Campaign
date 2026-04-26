---
share: true
tags:
  - character_sheet
  - crew
  - medtech
aliases:
lvlconversation: 5
lvleducation: 3
lvlevasion: 5
lvlparamedic: 6
locations:
  - "[[Watson]]"
  - "[Little China](little-china.md)"
luckincrement: 1
reputationincrement: 1
portrait: "[cover right circle hsmall wsmall lp](x-system-filesassetsimagescharacterscrewcrewdrtheory.png)"
character_type: Crew
totalhp: 10
totalhumanity: 0
seriouslywounded: 5
deathsave: 0
armourbodymelee: 0
armourheadmelee: 0
baseconcentration: 0
baseconcealreveal: 0
baselipreading: 0
baseperception: 0
basedrivelandvehicle: 0
basepilotairvehicle: 0
basepilotseavehicle: 0
baseriding: 0
baseaccounting: 0
baseanimalhandling: 0
basebureacracy: 0
basebuiness: 0
basecomposition: 0
basecriminology: 0
basecryptography: 0
basededuction: 0
baseeducation: 3
basegamble: 0
baselanguage: 0
baseenglish: 0
basestreetslang: 0
baselibrarysearch: 0
baselocalexpert: 0
baselittlechina: 0
basethestreets: 0
basetactics: 0
basewildernesssurvival: 0
basebrawling: 0
baseevasion: 5
basemartialarts: 0
basemeleeweapon: 0
baseathletics: 0
basecontortionist: 0
basedance: 0
baseendurance: 0
baseresisttorturedrugs: 0
basestealth: 0
basearchery: 0
baseautofire: 0
basehandgun: 0
baseheavyweapons: 0
baseshoulderarms: 0
basebribery: 0
baseconversation: 5
basehumanperception: 0
baseinterrogation: 0
basepersuasion: 0
basepersonalgrooming: 0
basestreetwise: 0
basetrading: 0
basewardrobestyle: 0
baseairvehicletech: 0
basebasictech: 0
basecybertech: 0
basedemolitions: 0
baseelectronics: 0
basefirstaid: 0
baseforgery: 0
baselandvehicletech: 0
basepaintdrawsculpt: 0
baseparamedic: 3
basephotographyfilm: 0
basepicklock: 0
basepickpocket: 0
baseseavehicletech: 0
baseweaponstech: 0
baseacting: 0
baseplayinstrument: 0
baseinstrument1: 0
currenthp: 10
currentluck: ""
currenthumanity: 0
---

> [!statblocks|wfit]
> ![cover right circle hsmall wsmall lp](x-system-filesassetsimagescharacterscrewcrewdrtheory.png)
> 
>```meta-bind-button
>style: "primary"
>label: "New Death Save"
>id: "deathsaveincrement"
>hidden: true
>action:
>    type: "updateMetadata"
>    bind_target "deathsavepenalty"
>    evaluate: true
>    value: "Math.min(x + 1, getMetadata('body'))"
>```
>```meta-bind-button
>style: "primary"
>label: "Reset DS Penalty"
>id: "deathsavereset"
>hidden: true
>action:
>    type: "updateMetadata"
>    bind_target "deathsavepenalty"
>    evaluate: true
>    value: "0"
>```
>```meta-bind-button
>style: "primary"
>label: "Reputation +"
>id: "reputationincrease"
>hidden: true
>action:
>    type: "updateMetadata"
>    bind_target "reputation"
>    evaluate: true
>    value: "Math.min(x + getMetadata('reputationincrement'), 10)"
>```
>```meta-bind-button
>style: "primary"
>label: "Reputation -"
>id: "reputationdecrease"
>hidden: true
>action:
>    type: "updateMetadata"
>    bind_target "reputation"
>    evaluate: true
>    value: "Math.max(x - getMetadata('reputationincrement'), 0)"
>```
>```meta-bind-button
>style: "primary"
>label: "Reputation Reset"
>id: "reputationreset"
>hidden: true
>action:
>    type: "updateMetadata"
>    bind_target "reputation"
>    evaluate: true
>    value: "0"
>```
>```meta-bind-button
>style: "primary"
>label: "HP +"
>id: "hpincrease"
>hidden: true
>action:
>    type: "updateMetadata"
>    bind_target "currenthp"
>    evaluate: true
>    value: "Math.min(x + getMetadata('hpincrement'), getMetadata('totalhp'))"
>```
>```meta-bind-button
>style: "primary"
>label: "HP -"
>id: "hpdecrease"
>hidden: true
>action:
>    type: "updateMetadata"
>    bind_target "currenthp"
>    evaluate: true
>    value: "Math.max(x - getMetadata('hpincrement'), 0)"
>```
>```meta-bind-button
>style: "primary"
>label: "HP Reset"
>id: "hpreset"
>hidden: true
>action:
>    type: "updateMetadata"
>    bind_target "currenthp"
>    evaluate: true
>    value: "getMetadata('totalhp')"
>```
>```meta-bind-button
>style: "primary"
>label: "Humanity +"
>id: "humanityincrease"
>hidden: true
>action:
>    type: "updateMetadata"
>    bind_target "currenthumanity"
>    evaluate: true
>    value: "Math.min(x + getMetadata('humanityincrement'), getMetadata('totalhumanity'))"
>```
>```meta-bind-button
>style: "primary"
>label: "Humanity -"
>id: "humanitydecrease"
>hidden: true
>action:
>    type: "updateMetadata"
>    bind_target "currenthumanity"
>    evaluate: true
>    value: "Math.max(x - getMetadata('humanityincrement'), 0)"
>```
>```meta-bind-button
>style: "primary"
>label: "Humanity Reset"
>id: "humanityreset"
>hidden: true
>action:
>    type: "updateMetadata"
>    bind_target "currenthumanity"
>    evaluate: true
>    value: "getMetadata('totalhumanity')"
>```
>```meta-bind-button
>style: "primary"
>label: "Luck -"
>id: "luckdecrease"
>hidden: true
>action:
>    type: "updateMetadata"
>    bind_target "currentluck"
>    evaluate: true
>    value: "Math.max(x - getMetadata('luckincrement'), 0)"
>```
>```meta-bind-button
>style: "primary"
>label: "Luck Reset"
>id: "luckreset"
>hidden: true
>action:
>    type: "updateMetadata"
>    bind_target "currentluck"
>    evaluate: true
>    value: "getMetadata('totalluck')"
>```
> # "Dr." Theory
> **Role**: [Medtech](medtech.md)
> *Role Ability*: Surgeon
> 
>> [!kith] Description
>> Dr Theory is a doctor, in theory. Homeless in [Night City](3-worldlocationsnorth-americanight-citynight-city.md) since deserting during the [Reunification War](reunification-war.md), Dr Theory learned his craft on the battlefield and proves it on the streets of [Little China](little-china.md).
>---
> 
>> [!info|title-center] Stats
>> | INT | REF | DEX | TECH | COOL | WILL | MOVE | BODY | EMP |
>> | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
>> | `INPUT[inlineSelect(defaultValue(1),option(1),option(2),option(3),option(4),option(5),option(6),option(7),option(8),option(9)):int]` | `INPUT[inlineSelect(defaultValue(1),option(1),option(2),option(3),option(4),option(5),option(6),option(7),option(8),option(9)):ref]` | `INPUT[inlineSelect(defaultValue(1),option(1),option(2),option(3),option(4),option(5),option(6),option(7),option(8),option(9)):dex]` | `INPUT[inlineSelect(defaultValue(1),option(1),option(2),option(3),option(4),option(5),option(6),option(7),option(8),option(9)):tech]` | `INPUT[inlineSelect(defaultValue(1),option(1),option(2),option(3),option(4),option(5),option(6),option(7),option(8),option(9)):cool]` | `INPUT[inlineSelect(defaultValue(1),option(1),option(2),option(3),option(4),option(5),option(6),option(7),option(8),option(9)):will]` | `INPUT[inlineSelect(defaultValue(1),option(1),option(2),option(3),option(4),option(5),option(6),option(7),option(8),option(9)):move]` | `INPUT[inlineSelect(defaultValue(1),option(1),option(2),option(3),option(4),option(5),option(6),option(7),option(8),option(9)):body]` | `INPUT[inlineSelect(defaultValue(1),option(1),option(2),option(3),option(4),option(5),option(6),option(7),option(8),option(9)):emp]` |
>> ---
>> | HP | Humanity | Luck | Reputation |
>> |:---:|:----------:|:-----:|:----------: |
>> | `VIEW[{currenthp}]` | `VIEW[{currenthumanity}]` | `VIEW[{currentluck}]` | |
>> | *out of* | *out of* | *out of* |  |
>> | **`VIEW[ceil(({body}+{will})/2)*5+10][math:totalhp]`** | **`VIEW[{emp}*10][math:totalhumanity]`** | **`INPUT[inlineSelect(defaultValue(1),option(1),option(2),option(3),option(4),option(5),option(6),option(7),option(8),option(9)):totalluck]`** | **`VIEW[{reputation}]`** |
>> 
>>> [!todo|title-center]- Stat Actions
>>>> [!blank|table]
>>>> |Amount| | | |
>>>> |:-:|:-:|:-:|:-:|
>>>> |`INPUT[number(title("HP")):hpincrement]`|`BUTTON[hpincrease]`|`BUTTON[hpdecrease]`|`BUTTON[hpreset]`|
>>>> |`INPUT[number:humanityincrement]`|`BUTTON[humanityincrease]`|`BUTTON[humanitydecrease]`|`BUTTON[humanityreset]`|
>>>> |`VIEW[1][math:luckincrement]`| |`BUTTON[luckdecrease]`|`BUTTON[luckreset]`|
>>>> |`VIEW[1][math:reputationincrement]`|`BUTTON[reputationincrease]`|`BUTTON[reputationdecrease]`|`BUTTON[reputationreset]`|
> 
>> [!danger|title-center]+ Death Saves
>> | Seriously Wounded at | Death Save Penalty | Death Save | |
>> | :-: | :-:| :-: | :-: |
>> | `VIEW[ceil({totalhp}/2)][math:seriouslywounded]` | `VIEW[max({deathsavepenalty},0)]` | `VIEW[{body}-max({deathsavepenalty},0)][math:deathsave]` | `BUTTON[deathsavereset]`|
>>
>>| |
>>|:-:|
>>|`BUTTON[deathsaveincrement]`|
> 
>>[!abstract|title-center clean]- Armour and Attacks
>>>[!blank|table wfit]
>>> | Armour | Body | Head |
>>> | -------: | :----: | :----: |
>>> | vs Ranged/Brawl | `INPUT[number:armourbodyranged]` | `INPUT[number:armourheadranged]` |
>>> | vs Melee/M.Art | `VIEW[ceil({armourbodyranged}/2)][math:armourbodymelee]` | `VIEW[ceil({armourheadranged}/2)][math:armourheadmelee]` |
>>> ---
>>> | Weapon | Skill | Base | DMG | Ammo | ROF | One Handed | Concealable |
>>> | -------: | ----: | :----: | :----: | :-----: | :----: | :------------: | :-----------: |
>>> | Rifle | Shoulder Arms | 1d10+12 | 5d6 | 4 | 1 | N | N |
> 
>> [!abstract|title-center clean]- Skills
>> **Total level points spent:** `VIEW[{lvlconcentration} + {lvlconcealreveal} + {lvllipreading} + {lvlperception} + {lvltracking} + {lvldrivelandvehicle} + {lvlpilotairvehicle} + {lvlpilotseavehicle} + {lvlriding} + {lvlaccounting} + {lvlanimalhandling} + {lvlbureaucracy} + {lvlbusiness} + {lvlcomposition} + {lvlcriminology} + {lvlcryptography} + {lvldeduction} + {lvleducation} + {lvlgamble} + {lvllanguage} + {lvllibrarysearch} + {lvllocalexpert} + {lvlscience} + {lvltactics} + {lvlwildernesssurvival} + {lvlbrawling} + {lvlevasion} + {lvlmartialarts} + {lvlmeleeweapon} + {lvlathletics} + {lvlcontortionist} + {lvldance} + {lvlendurance} + {lvlresisttorturedrugs} + {lvlstealth} + {lvlarchery} + {lvlautofire} + {lvlhandgun} + {lvlheavyweapons} + {lvlshoulderarms} + {lvlbribery} + {lvlconversation} + {lvlhumanperception} + {lvlinterrogation} + {lvlpersuasion} + {lvlpersonalgrooming} + {lvlstreetwise} + {lvltrading} + {lvlwardrobestyle} + {lvlairvehicletech} + {lvlbasictech} + {lvlcybertech} + {lvldemolitions} + {lvlelectronics} + {lvlfirstaid} + {lvlforgery} + {lvllandvehicletech} + {lvlpaintdrawsculpt} + {lvlparamedic} + {lvlphotographyfilm} + {lvlpicklock} + {lvlpickpocket} + {lvlseavehicletech} + {lvlweaponstech} + {lvlacting} + {lvlplayinstrument}]` / 90
>>> [!columns|2 no-t table table-wide]
>>>> | | Stat | Level | Base |
>>>> | --: | --: | :-: | :-: | 
>>>> | **Awareness Skills** | | | |
>>>> | Concentration | WILL `VIEW[{will}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlconcentration]` | `VIEW[{will}+{lvlconcentration}][math:baseconcentration]` |
>>>> | Conceal/Reveal | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlconcealreveal]` | `VIEW[{int}+{lvlconcealreveal}][math:baseconcealreveal]` |
>>>> | Lipreading | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvllipreading]` | `VIEW[{int}+{lvllipreading}][math:baselipreading]`  |
>>>> | Perception | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlperception]` | `VIEW[{int}+{lvlperception}][math:baseperception]`  |
>>>> | Tracking | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvltracking]` | `VIEW[{int}+{lvllipreading}][math:baselipreading]`  |
>>>> | **Control Skills** | | | |
>>>> | Drive Land Vehicle | REF `VIEW[{ref}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvldrivelandvehicle]` | `VIEW[{ref}+{lvldrivelandvehicle}][math:basedrivelandvehicle]`  |
>>>> | Pilot Air Vehicle (x2) | REF `VIEW[{ref}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlpilotairvehicle]` | `VIEW[{ref}+floor({lvlpilotairvehicle}/2)][math:basepilotairvehicle]` |
>>>> | Pilot Sea Vehicle | REF `VIEW[{ref}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlpilotseavehicle]` | `VIEW[{ref}+{lvlpilotseavehicle}][math:basepilotseavehicle]` |
>>>> | Riding | REF `VIEW[{ref}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlriding]` | `VIEW[{ref}+{lvlriding}][math:baseriding]` |
>>>> | **Education Skills** | | | |
>>>> | Accounting | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlaccounting]` | `VIEW[{int}+{lvlaccouting}][math:baseaccounting]` |
>>>> | Animal Handling | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlanimalhandling]` | `VIEW[{int}+{lvlanimalhandling}][math:baseanimalhandling]` |
>>>> | Bureaucracy | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlbureaucracy]` | `VIEW[{int}+{lvlbureaucracy}][math:basebureacracy]` |
>>>> | Business | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlbusiness]` | `VIEW[{int}+{lvlbuiness}][math:basebuiness]` |
>>>> | Composition | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlcomposition]` | `VIEW[{int}+{lvlcomposition}][math:basecomposition]` |
>>>> | Criminology | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlcriminology]` | `VIEW[{int}+{lvlcriminology}][math:basecriminology]` |
>>>> | Cryptography | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlcryptography]` | `VIEW[{int}+{lvlcryptography}][math:basecryptography]` |
>>>> | Deduction | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvldeduction]` | `VIEW[{int}+{lvldeduction}][math:basededuction]` |
>>>> | Education | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvleducation]` | `VIEW[{int}+{lvleducation}][math:baseeducation]` |
>>>> | Gamble | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlgamble]` | `VIEW[{int}+{lvlgamble}][math:basegamble]` |
>>>> | Language | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvllanguage]` | `VIEW[{int}+{lvllanguage}][math:baselanguage]` |
>>>> | *[English](english.md)↵* | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlenglish]` | `VIEW[{int}+{lvlenglish}][math:baseenglish]` |
>>>> | *[Streetslang](streetslang.md)↵* | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlstreetslang]` | `VIEW[{int}+{lvlstreetslang}][math:basestreetslang]` |
>>>> | Library Search | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvllibrarysearch]` | `VIEW[{int}+{lvllibrarysearch}][math:baselibrarysearch]` |
>>>> | Local Expert | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvllocalexpert]` | `VIEW[{int}+{lvllocalexpert}][math:baselocalexpert]` |
>>>> | *[Little China](little-china.md)↵* | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvllittlechina]` | `VIEW[{int}+{lvllittlechina}][math:baselittlechina]` |
>>>> | *The Streets↵* | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlthestreets]` | `VIEW[{int}+{lvlthestreets}][math:basethestreets]` |
>>>> | Tactics | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvltactics]` | `VIEW[{int}+{lvltactics}][math:basetactics]` |
>>>> | Wilderness Survival | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlwildernesssurvival]` | `VIEW[{int}+{lvlwildernesssurvival}][math:basewildernesssurvival]` |
>>>> | **Fighting Skills** | | | |
>>>> | Brawling | DEX `VIEW[{dex}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlbrawling]` | `VIEW[{dex}+{lvlbrawling}][math:basebrawling]` |
>>>> | Evasion | DEX `VIEW[{dex}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlevasion]` | `VIEW[{dex}+{lvlevasion}][math:baseevasion]` |
>>>> | Martial Arts (x2) | DEX `VIEW[{dex}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlmartialarts]` | `VIEW[{dex}+floor({lvlmartialarts}/2)][math:basemartialarts]` |
>>>> | Melee Weapon | DEX `VIEW[{dex}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlmeleeweapon]` | `VIEW[{dex}+{lvlmeleeweapon}][math:basemeleeweapon]` |
>>>
>>>> | | Stat | Level | Base |
>>>> | --: | --: | :-: | :-: | 
>>>> | **Body Skills** | | | |
>>>> | Athletics | DEX `VIEW[{dex}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlathletics]` | `VIEW[{dex}+{lvlathletics}][math:baseathletics]` |
>>>> | Contortionist | DEX `VIEW[{dex}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlcontortionist]` | `VIEW[{dex}+{lvlcontortionist}][math:basecontortionist]` |
>>>> | Dance | DEX `VIEW[{dex}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvldance]` | `VIEW[{dex}+{lvldance}][math:basedance]` |
>>>> | Endurance | WILL `VIEW[{will}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlendurance]` | `VIEW[{will}+{lvlendurance}][math:baseendurance]` |
>>>> | Resist Torture/Drugs | WILL `VIEW[{will}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlresisttorturedrugs]` | `VIEW[{will}+{lvlresisttorturedrugs}][math:baseresisttorturedrugs]` |
>>>> | Stealth | DEX `VIEW[{dex}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlstealth]` | `VIEW[{dex}+{lvlstealth}][math:basestealth]` |
>>>> | **Ranged  Weapon Skills** | | | |
>>>> | Archery | REF `VIEW[{ref}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlarchery]` | `VIEW[{ref}+{lvlarchery}][math:basearchery]` |
>>>> | Autofire (x2) | REF `VIEW[{ref}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlautofire]` | `VIEW[{ref}+floor({lvlautofire}/2)][math:baseautofire]` |
>>>> | Handgun | REF `VIEW[{ref}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlhandgun]` | `VIEW[{ref}+{lvlhandgun}][math:basehandgun]` |
>>>> | Heavy Weapons (x2) | REF `VIEW[{ref}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlheavyweapons]` | `VIEW[{ref}+floor({lvlheavyweapons}/2)][math:baseheavyweapons]` |
>>>> | Shoulder Arms | REF `VIEW[{ref}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlshoulderarms]` | `VIEW[{ref}+{lvlshoulderarms}][math:baseshoulderarms]` |
>>>> | **Social Skills** | | | |
>>>> | Bribery | COOL `VIEW[{cool}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlbribery]` | `VIEW[{cool}+{lvlbribery}][math:basebribery]` |
>>>> | Conversation | EMP `VIEW[{emp}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlconversation]` | `VIEW[{emp}+{lvlconversation}][math:baseconversation]` |
>>>> | Human Perception | EMP `VIEW[{emp}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlhumanperception]` | `VIEW[{emp}+{lvlhumanperception}][math:basehumanperception]` |
>>>> | Interrogation | COOL `VIEW[{cool}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlinterrogation]` | `VIEW[{cool}+{lvlinterrogation}][math:baseinterrogation]` |
>>>> | Persuasion | COOL `VIEW[{cool}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlpersuasion]` | `VIEW[{cool}+{lvlpersuasion}][math:basepersuasion]` |
>>>> | Personal Grooming | COOL `VIEW[{cool}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlpersonalgrooming]` | `VIEW[{cool}+{lvlpersonalgrooming}][math:basepersonalgrooming]` |
>>>> | Streetwise | COOL `VIEW[{cool}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlstreetwise]` | `VIEW[{cool}+{lvlstreetwise}][math:basestreetwise]` |
>>>> | Trading | COOL `VIEW[{cool}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvltrading]` | `VIEW[{cool}+{lvltrading}][math:basetrading]` |
>>>> | Wardrobe & Style | COOL `VIEW[{cool}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlwardrobestyle]` | `VIEW[{cool}+{lvlwardrobestyle}][math:basewardrobestyle]` |
>>>> | **Technique Skills** | | | |
>>>> | Air Vehicle Tech | TECH `VIEW[{tech}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlairvehicletech]` | `VIEW[{tech}+{lvlairvehicletech}][math:baseairvehicletech]` |
>>>> | Basic Tech | TECH `VIEW[{tech}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlbasictech]` | `VIEW[{tech}+{lvlbasictech}][math:basebasictech]` |
>>>> | Cybertech | TECH `VIEW[{tech}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlcybertech]` | `VIEW[{tech}+{lvlcybertech}][math:basecybertech]` |
>>>> | Demolitions (x2) | TECH `VIEW[{tech}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvldemolitions]` | `VIEW[{tech}+floor({lvldemolitions}/2)][math:basedemolitions]` |
>>>> | Electronics (x2) | TECH `VIEW[{tech}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlelectronics]` | `VIEW[{tech}+floor({lvlelectronics}/2)][math:baseelectronics]` |
>>>> | First Aid | TECH `VIEW[{tech}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlfirstaid]` | `VIEW[{tech}+{lvlfirstaid}][math:basefirstaid]` |
>>>> | Forgery | TECH `VIEW[{tech}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlforgery]` | `VIEW[{tech}+{lvlforgery}][math:baseforgery]` |
>>>> | Land Vehicle Tech | TECH `VIEW[{tech}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvllandvehicletech]` | `VIEW[{tech}+{lvllandvehicletech}][math:baselandvehicletech]` |
>>>> | Paint/Draw/Sculpt | TECH `VIEW[{tech}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlpaintdrawscuplt]` | `VIEW[{tech}+{lvlpaintdrawsculpt}][math:basepaintdrawsculpt]` |
>>>> | Paramedic (x2) | TECH `VIEW[{tech}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlparamedic]` | `VIEW[{tech}+floor({lvlparamedic}/2)][math:baseparamedic]` |
>>>> | Photography/Film | TECH `VIEW[{tech}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlphotographyfilm]` | `VIEW[{tech}+{lvlphotographyfilm}][math:basephotographyfilm]` |
>>>> | Pick Lock | TECH `VIEW[{tech}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlpicklock]` | `VIEW[{tech}+{lvlpicklock}][math:basepicklock]` |
>>>> | Pick Pocket | TECH `VIEW[{tech}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlpickpocket]` | `VIEW[{tech}+{lvlpickpocket}][math:basepickpocket]` |
>>>> | Sea Vehicle Tech | TECH `VIEW[{tech}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlseavehicletech]` | `VIEW[{tech}+{lvlseavehicletech}][math:baseseavehicletech]` |
>>>> | Weapons Tech | TECH `VIEW[{tech}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlweaponstech]` | `VIEW[{tech}+{lvlweaponstech}][math:baseweaponstech]` |
>>>> | **Performance Skills** | | | |
>>>> | Acting | COOL `VIEW[{cool}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlacting]` | `VIEW[{cool}+{lvlacting}][math:baseacting]` |
>>>> | Play Instrument | TECH `VIEW[{tech}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlplayinstrument]` | `VIEW[{tech}+{lvlplayinstrument}][math:baseplayinstrument]` |
>>>> | *instrument↵* | TECH `VIEW[{tech}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlinstrument1]` | `VIEW[{tech}+{lvlinstrument1}][math:baseinstrument1]` |
>>>>
>>>>`VIEW[max({reputation}, 0)][math(hidden)]`
>>>>`VIEW[{totalhp}][math(hidden):currenthp]`
>>>>`VIEW[{totalluck}][math(hidden):currentluck]`
>>>>`VIEW[{totalhumanity}][math(hidden):currenthumanity]`


## Overview
Full name: Unknown
Class: [Medtech](medtech.md)
Subclass: Surgeon
Background: [Oceania](oceania.md)/[Australia](australia.md)
Personality: Paranoid, addicted, somewhat nuts
Values: Money
Cares for: [Dog](dr-theorys-dog.md), deceased, in pieces
Prized Possession: [Dog heart in pickle jar](dr-theorys-dog-heart.md)
Style: [Bagman](bagman.md)
Feelings about people: They are untrustworthy
## Relationships
[Character Sheet - Crash](character-sheet-crash.md) - Dr. Theory knows [Character Sheet - Crash](character-sheet-crash.md) after he sold her drugs while she was playing a gig under an overpass. He has continued to be her plug but they are otherwise friends.

## Character Background
Dr Theory left [Australia](australia.md) to fight in corporate wars. He served as a medic until the [Reunification War](reunification-war.md), at which point he deserted in [Night City](3-worldlocationsnorth-americanight-citynight-city.md).
The so-called "Dr." Theory (a doctor only in theory), now homeless in [Little China](little-china.md), practices street surgery without a license or formal education: the only permanent possessions of his are the remains of his [dog](dr-theorys-dog.md), pieces of which he wears in his coat and strung around his neck. His prized possession is the [dog's heart](dr-theorys-dog-heart.md), which he keeps in a pickle jar.

Dr Theory has an ongoing rivalry (one-sided) with all doctors, who he sees as sell-outs and hacks. Individually, these doctors do not know he exists.

He is paranoid that a government or corporate official is out to get him for deserting in the [Reunification War](reunification-war.md): Dr Theory is however face-blind, and while he swears the individual after him is a *particular* government or corporate official, he does not recognise that any given corporate or government official is not the person after him.