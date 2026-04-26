---
share: true
tags:
  - location
  - city_center
  - downtown
aliases:
parent_location: "[City Center](city-center.md)"
bordering_locations:
  - "[[Corporate Plaza]]"
  - "[[Wellsprings]]"
  - "[[Little China]]"
location_type: Neighbourhood
---

>[!infobox|wsmall wikipedia left]
># Downtown
>![wsmall cover](insertimage.png)
>
>## Info
>|||
>|--:|:--|
>|Type:|Neighbourhood|
>|Located In:|[City Center](city-center.md)|
>|Prestige:|High|
>---
>### Borders
> | Location                                                                                       | Location Type |
> | ---------------------------------------------------------------------------------------------- | ------------- |
> | [Little China](watsonlittle-china.md)            | Sub-District  |
> | [Wellsprings](heywoodwellsprings.md)             | Neighbourhood |
> | [Corporate Plaza](corporate-plaza.md) | Neighbourhood |
> | [Watson](watson.md)                               | District      |
> | [Heywood](heywood.md)                             | District      |
> 

# Summary
Downtown is a neighbourhood on the west side of the [City Center](city-center.md), in the middle of [Night City](night-city.md).

# History
- [2074-02-19 17.00 - ADOS Intro](2074-02-19-1700-ados-intro.md)


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
| [Angel Rosemont](characterscrewangel-rosemont.md) | ![100](x-system-filesassetsimagescharacterscrewcrewadossticker.png) | Crew           | <ul><li>[ZetaTech](3-worldfactionscorpszetatechmd.md)</li><li>[Crew](3-worldfactionscrewmd.md)</li></ul> |


# Gangs
| Gang | Danger Level | Operating Locations |
| ---- | ------------ | ------------------- |


# Map
![cover](mapcitycenter2077.png)