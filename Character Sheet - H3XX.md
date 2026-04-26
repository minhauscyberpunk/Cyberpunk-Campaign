---
share: true
tags:
  - character_sheet
  - crew
  - netrunner
aliases:
lvleducation: 4
lvlevasion: 6
basecorpo: 0
locations:
  - "[[Watson]]"
  - "[Little China](little-china.md)"
  - "[[H3XX's Apartment]]"
luckincrement: 1
reputationincrement: 1
baseeducation: 4
baseevasion: 6
portrait: "[cover right circle hsmall wsmall lp](x-system-filesassetsimagescharacterscrewcrewh3xx.png)"
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
basegamble: 0
baselanguage: 0
baseenglish: 0
basespanish: 0
basestreetslang: 0
baselibrarysearch: 0
baselocalexpert: 0
baselittlechina: 0
basecombatzones: 0
basescience: 0
basetactics: 0
basewildernesssurvival: 0
basebrawling: 0
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
baseconversation: 0
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
baseparamedic: 0
basephotographyfilm: 0
basepicklock: 0
basepickpocket: 0
baseseavehicletech: 0
baseweaponstech: 0
baseacting: 0
baseplayinstrument: 0
currenthp: 10
currentluck: ""
currenthumanity: 0
---

> [!statblocks|wfit]
> ![cover right circle hsmall wsmall lp](x-system-filesassetsimagescharacterscrewcrewh3xx.png)
> 
>```meta-bind-button
>style: "primary"
>label: "New Death Save"
>id: "deathsaveincrement"
>hidden: true
>action:
>    type: "updateMetadata"
>    bindTarget: "deathsavepenalty"
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
>    bindTarget: "deathsavepenalty"
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
>    bindTarget: "reputation"
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
>    bindTarget: "reputation"
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
>    bindTarget: "reputation"
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
>    bindTarget: "currenthp"
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
>    bindTarget: "currenthp"
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
>    bindTarget: "currenthp"
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
>    bindTarget: "currenthumanity"
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
>    bindTarget: "currenthumanity"
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
>    bindTarget: "currenthumanity"
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
>    bindTarget: "currentluck"
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
>    bindTarget: "currentluck"
>    evaluate: true
>    value: "getMetadata('totalluck')"
>```
> # H3XX
> **Role**: [Netrunner](netrunner.md)
> *Role Ability*:
> 
>> [!kith] Description
>> H3XX is a flashy [Netrunner](netrunner.md) out to prove herself. She signs all her hacks with bright flashy malware, much to the chagrin of her employers who often want her to keep a low profile. Nobody can argue that she doesn't get results, though: H3XX is a talented runner who wants everyone across the Net to know her name.
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
>>> | - | - | - | - | - | -| - | - |
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
>>>> | *[Spanish](spanish.md)↵* | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlspanish]` | `VIEW[{int}+{lvlspanish}][math:basespanish]` |
>>>> | *[Streetslang](streetslang.md)↵* | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlstreetslang]` | `VIEW[{int}+{lvlstreetslang}][math:basestreetslang]` |
>>>> | Library Search | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvllibrarysearch]` | `VIEW[{int}+{lvllibrarysearch}][math:baselibrarysearch]` |
>>>> | Local Expert | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvllocalexpert]` | `VIEW[{int}+{lvllocalexpert}][math:baselocalexpert]` |
>>>> | *[Little China](little-china.md)↵* | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvllittlechina]` | `VIEW[{int}+{lvllittlechina}][math:baselittlechina]` |
>>>> | *Old [Combat Zone](combat-zone.md)s↵* | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlcombatzones]` | `VIEW[{int}+{lvlcombatzones}][math:basecombatzones]` |
>>>> | *Corpo↵* | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlcorpo]` | `VIEW[{int}+{lvlcorpo}][math:basecorpo]` |
>>>> | Science | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlscience]` | `VIEW[{int}+{lvlscience}][math:basescience]` |
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
>>>>
>>>>`VIEW[max({reputation}, 0)][math(hidden)]`
>>>>`VIEW[{totalhp}][math(hidden):currenthp]`
>>>>`VIEW[{totalluck}][math(hidden):currentluck]`
>>>>`VIEW[{totalhumanity}][math(hidden):currenthumanity]`


## Overview
Full name: Unknown
Class: [Netrunner](netrunner.md)
Subclass:
Background: [North America](north-america.md)/[Mexico](mexico.md)
Personality: Desperate for approval
Values: Her image/reputation
Cares for: A mentor
Prized Possession: Boots
Style: [Asia Pop](asia-pop.md)
Feelings about people: They are untrustworthy
## Relationships
- [Character Sheet - Asher](character-sheet-asher.md): H3XX has worked jobs with [Character Sheet - Asher](character-sheet-asher.md) in the past for Corpos in [Charter Hill](charter-hill.md) and [North Oak](north-oak.md). The two get along well enough, but [Character Sheet - Asher](character-sheet-asher.md) does believe that H3XX is unprofessional on the job.
- [Character Sheet - ADOS](character-sheet-ados.md): H3XX is aware of [Character Sheet - ADOS](character-sheet-ados.md) by reputation as a [Netrunner](netrunner.md): she is unaware that [Character Sheet - ADOS](character-sheet-ados.md) is Angel Rosemont, daughter of the [ZetaTech](zetatech.md) CEO.

## Character Background
H3XX grew up in a [Combat Zone](combat-zone.md) in [Night City](3-worldlocationsnorth-americanight-citynight-city.md) (in what *used* to be quite a nice neighbourhood) at the end of the [Time of the Red](time-of-the-red.md). She learned to hack and netrun using scavenged [Cyberdeck](cyberdeck.md)s. Her parents were killed in the [Combat Zone](combat-zone.md) when she was young, and she has come to rely on only herself and her reputation to stay alive.

She has done relatively well for herself doing gigs for Corpos in [Charter Hill](charter-hill.md) and [North Oak](north-oak.md), including hacking, cybersecurity, comms, and assisting in more complex jobs such as bodyguarding. She lives in a small apartment in [Little China](little-china.md), which is completely loaded with brightly coloured and decorated tech and netrunning equipment.

She signs all her hacks with signature pop-up ads: her employers often wish she wouldn't do this, as discretion is often required. Nonetheless, her skills are good and she is in relatively high demand as a [Netrunner](netrunner.md).