---
share: true
tags:
  - location
  - city_center
  - downtown
aliases:
parent_location: "[[City Center]]"
bordering_locations:
  - "[[Corporate Plaza]]"
  - "[[Wellsprings]]"
  - "[[Little China]]"
location_type: Neighbourhood
---

>[!infobox|wsmall wikipedia left]
># Downtown
>![[insert_image.png|wsmall cover]]
>
>## Info
>|||
>|--:|:--|
>|Type:|Neighbourhood|
>|Located In:|[[City Center]]|
>|Prestige:|High|
>---
>### Borders
> | Location                                                                                       | Location Type |
> | ---------------------------------------------------------------------------------------------- | ------------- |
> | [[3 World/Locations/North America/Night City/Watson/Little China.md\|Little China]]            | Sub-District  |
> | [[3 World/Locations/North America/Night City/Heywood/Wellsprings.md\|Wellsprings]]             | Neighbourhood |
> | [[3 World/Locations/North America/Night City/City Center/Corporate Plaza.md\|Corporate Plaza]] | Neighbourhood |
> | [[3 World/Locations/North America/Night City/Watson.md\|Watson]]                               | District      |
> | [[3 World/Locations/North America/Night City/Heywood.md\|Heywood]]                             | District      |
> 

# Summary
Downtown is a neighbourhood on the west side of the [[City Center]], in the middle of [[Night City|Night City]].

# History
- [[5 Sessions/Our Story/Beat Planning/2074-02-19 The Intro Job - August’s Data Chip/2074-02-19 17.00 - ADOS Intro.md|2074-02-19 17.00 - ADOS Intro]]


# Notable Places

```meta-bind-button
style: "primary"
label: "Create New Sub-Location"
id: "createSubLocation"
action:
  type: js
  file: X System Files/User Scripts/newLocation.js
  args:
    dest_folder: destFolder
```
|  |
|  |
dataview
TABLE WITHOUT ID file.link AS "Location", location_type AS "Location Type"
FROM #location 
WHERE parent_location = this.file.link
SORT location_type DESC, file.link ASC
```
```

# Notable Characters
| Character                                                     |                                                                             | Character Type | Factions                                                                                                        |
| ------------------------------------------------------------- | --------------------------------------------------------------------------- | -------------- | --------------------------------------------------------------------------------------------------------------- |
| [[3 World/Characters/Crew/Angel Rosemont.md\|Angel Rosemont]] | ![[X System Files/Assets/Images/Characters/Crew/CrewADOS_sticker.png\|100]] | Crew           | <ul><li>[[3 World/Factions/Corps/ZetaTech.md\|ZetaTech]]</li><li>[[3 World/Factions/Crew.md\|Crew]]</li></ul> |


# Gangs
| Gang | Danger Level | Operating Locations |
| ---- | ------------ | ------------------- |


# Map
![[MapCityCenter2077.png|cover]]