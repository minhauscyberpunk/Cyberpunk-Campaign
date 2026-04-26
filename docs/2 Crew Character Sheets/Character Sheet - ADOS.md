---
share: true
tags:
  - character_sheet
  - crew
  - netrunner
aliases:
lvlconversation: 6
lvleducation: 6
basecorpo: 0
lvlnorthoaks: 0
locations:
  - "[[Westbrook]]"
  - "[North Oak](../3%20World/Locations/North%20America/Night%20City/Westbrook/North%20Oak.md)"
  - "[[Rosemont House]]"
luckincrement: 1
reputationincrement: 1
baseeducation: 6
basenorthoaks: 0
baseconversation: 6
portrait: "[cover right circle hsmall wsmall lp](../X%20System%20Files/Assets/Images/Characters/Crew/CrewADOS.png)"
character_type: Crew
factions:
  - "[ZetaTech](../3%20World/Factions/Corps/ZetaTech.md)"
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
basefrench: 0
basestreetslang: 0
baselibrarysearch: 0
baselocalexpert: 0
baselittlechina: 0
basescience: 0
basetactics: 0
basewildernesssurvival: 0
basebrawling: 0
baseevasion: 0
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
> ![cover right circle hsmall wsmall lp](../X%20System%20Files/Assets/Images/Characters/Crew/CrewADOS.png)
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
> # ADOS
> **Role**: [Netrunner](../4%20Rules%20and%20Mechanics/Roles/Netrunner.md)
> *Role Ability*:
> 
>> [!kith] Description
>> Angel Rosemont, scion of the [ZetaTech](../3%20World/Factions/Corps/ZetaTech.md) corporation, moonlights as the [Netrunner](../4%20Rules%20and%20Mechanics/Roles/Netrunner.md), ADOS. Fresh out of school and taking a year's sabbatical to gain experience, will Angel return to the fold as an experienced corporate runner/exec, or will she get chewed up by [Night City](3%20World/Locations/North%20America/Night%20City/Night%20City.md) and spat out as ADOS?
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
>>> | V.H.Pistol | Handgun | 11 | 4d6 | 8 | 1 | Y | N |
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
>>>> | *[English](../4%20Rules%20and%20Mechanics/Languages/English.md)↵* | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlenglish]` | `VIEW[{int}+{lvlenglish}][math:baseenglish]` |
>>>> | *[French](../4%20Rules%20and%20Mechanics/Languages/French.md)↵* | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlfrench]` | `VIEW[{int}+{lvlfrench}][math:basefrench]` |
>>>> | *[Streetslang](../4%20Rules%20and%20Mechanics/Languages/Streetslang.md)↵* | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlstreetslang]` | `VIEW[{int}+{lvlstreetslang}][math:basestreetslang]` |
>>>> | Library Search | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvllibrarysearch]` | `VIEW[{int}+{lvllibrarysearch}][math:baselibrarysearch]` |
>>>> | Local Expert | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvllocalexpert]` | `VIEW[{int}+{lvllocalexpert}][math:baselocalexpert]` |
>>>> | *[Little China](../3%20World/Locations/North%20America/Night%20City/Watson/Little%20China.md)↵* | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvllittlechina]` | `VIEW[{int}+{lvllittlechina}][math:baselittlechina]` |
>>>> | *[North Oak](../3%20World/Locations/North%20America/Night%20City/Westbrook/North%20Oak.md)↵* | INT `VIEW[{int}]` | `INPUT[inlineSelect(defaultValue(0),option(0),option(1),option(2),option(3),option(4),option(5),option(6)):lvlnorthoaks]` | `VIEW[{int}+{lvlnorthoaks}][math:basenorthoaks]` |
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
Full name: Angel Rosemont
Class: [Netrunner](../4%20Rules%20and%20Mechanics/Roles/Netrunner.md)
Subclass: unknown
Background: unknown
Personality: unknown
Values: unknown
Cares for: unknown
Prized Possession: unknown
Style: unknown
Feelings about people: unknown
## Relationships
[Character Sheet - H3XX](./Character%20Sheet%20-%20H3XX.md) - ADOS is aware of H3XX by reputation, and also that H3XX has worked for [ZetaTech](../3%20World/Factions/Corps/ZetaTech.md) in the past.
[Character Sheet - Crash](./Character%20Sheet%20-%20Crash.md) - Childhood rival/enemy
## Provided Character Background
As the only daughter of two [ZetaTech](../3%20World/Factions/Corps/ZetaTech.md) executives, Angel has never gone without absolute luxury and comfort. [Eddies](../4%20Rules%20and%20Mechanics/Dictionary/Eddies.md) talks in these circles, and what her parents couldn't offer her in love or affection, they paid tenfold in money. A private wing in her family's [North Oak](../3%20World/Locations/North%20America/Night%20City/Westbrook/North%20Oak.md) estate and a full staff of attendants was to be expected, of course. But with such a prestigious family, Angel never truly had a choice in her career or life. Pushed into the family business from her youth, she was writing code before she could even read what it said. As a result of her conditioning and augmentations, she quickly became an adept software developer. But there was no fun in that for her, no excitement to be had.
Her real passion lied in netrunning - unleashing daemons on bothersome classmates or draining someone's bank account. Not for the money, merely for the thrill that she could.
She began living a second life. There was Miss Angel Rosemont, the charming yet manipulative heir apparent to a large fortune and future executive of [ZetaTech](../3%20World/Factions/Corps/ZetaTech.md). Then there was ADOS, a cunning and meticulous [Netrunner](../4%20Rules%20and%20Mechanics/Roles/Netrunner.md) that fixers began to catch wind of. She started taking up odd jobs as ADOS, stealing compromising and embarrassing files of various celebrities, or fucking with rival companies to drag down their stock prices. Angel knew of these targets in a personal capacity, some of her targets were even close family friends. She got a kick out of knowing their secrets or seeing their professional lives take a hit. Life to her is a struggle for knowledge, and there is this satisfaction in having an advantage over someone else that drives her to continue.
She is scheming, strategic and ruthless, a real diplomat. Angel is a respectable young woman, of course, so any suggestion of her second life as ADOS would be laughable on its face. She is fundamentally naive, however, she's never really faced any real threat to her life or god forbid, her reputation. She has never had any reason to take on any kind of physical fight, so she is woefully unprepared in genuine combat. She's used to working alone as ADOS, but networking is a core part of her life as Angel, so she could easily work with a team if that was beneficial to her. She wouldn't try to run the operation, merely to do her role and observe from the sidelines, influencing with her charm as opposed to intimidating or blackmail. She does a good job of covering her tracks as a saboteur, but if she's worked her magic on you, you've never even thought to question that there is anything deeper to her. But if her web of lies and deceit began to untangle, her natural wit and allure might not be enough to save her.
She stands now at a crossroad. She's taken a sabbatical after graduating high school, ostensibly to develop her professional relationships but it's really to give her more time deepening her connections with fixers and building her resumè as a reliable runner. Once the year is over however, Angel will be swept into [ZetaTech](../3%20World/Factions/Corps/ZetaTech.md) in some bullshit managerial role. But maybe her flirting with the illicit world of hacking for hire will see her shunned from her family, in hiding, or scrapped for augments and left dead in some alleyway? Or maybe ADOS will be headhunted for intelligence, and have the chance to turn this side thing into a career with the resources to match her ambition.