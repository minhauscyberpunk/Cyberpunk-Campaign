---
share: true
tags:
  - location
  - city_center
  - downtown
aliases:
parent_location: "[City Center](../City%20Center.md)"
bordering_locations:
  - "[[Corporate Plaza]]"
  - "[[Wellsprings]]"
  - "[[Little China]]"
location_type: Neighbourhood
---

>[!infobox|wsmall wikipedia left]
># Downtown
>![wsmall cover](insert_image.png)
>
>## Info
>|||
>|--:|:--|
>|Type:|Neighbourhood|
>|Located In:|[City Center](../City%20Center.md)|
>|Prestige:|High|
>---
>### Borders
> | Location                                                                                       | Location Type |
> | ---------------------------------------------------------------------------------------------- | ------------- |
> | [Little China](../Watson/Little%20China.md)            | Sub-District  |
> | [Wellsprings](../Heywood/Wellsprings.md)             | Neighbourhood |
> | [Corporate Plaza](./Corporate%20Plaza.md) | Neighbourhood |
> | [Watson](../Watson.md)                               | District      |
> | [Heywood](../Heywood.md)                             | District      |
> 

# Summary
Downtown is a neighbourhood on the west side of the [City Center](../City%20Center.md), in the middle of [Night City](../../Night%20City.md).

# History
- [2074-02-19 17.00 - ADOS Intro](../../../../../../2074-02-19%2017.00%20-%20ADOS%20Intro.md)


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
| [Angel Rosemont](../../../../Characters/Crew/Angel%20Rosemont.md) | ![100](../../../../../X%20System%20Files/Assets/Images/Characters/Crew/CrewADOS_sticker.png) | Crew           | <ul><li>[ZetaTech](3%20World/Factions/Corps/ZetaTech.md.md)</li><li>[Crew](3%20World/Factions/Crew.md.md)</li></ul> |


# Gangs
| Gang | Danger Level | Operating Locations |
| ---- | ------------ | ------------------- |


# Map
![cover](MapCityCenter2077.png)