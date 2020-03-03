---
title: "conditionalAccessConditionSet resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# conditionalAccessConditionSet resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|applications|[conditionalAccessApplications](../resources/conditionalaccessapplications.md)||
|clientAppTypes|Enumeration collection||
|deviceStates|[conditionalAccessDeviceStates](../resources/conditionalaccessdevicestates.md)||
|locations|[conditionalAccessLocations](../resources/conditionalaccesslocations.md)||
|platforms|[conditionalAccessPlatforms](../resources/conditionalaccessplatforms.md)||
|signInRiskLevels|Enumeration collection||
|users|[conditionalAccessUsers](../resources/conditionalaccessusers.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conditionalAccessConditionSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conditionalAccessConditionSet",
  "applications": {
    "@odata.type": "microsoft.graph.conditionalAccessApplications",
    "includeApplications": [
      "String"
    ],
    "excludeApplications": [
      "String"
    ],
    "includeUserActions": [
      "String"
    ]
  },
  "users": {
    "@odata.type": "microsoft.graph.conditionalAccessUsers",
    "includeUsers": [
      "String"
    ],
    "excludeUsers": [
      "String"
    ],
    "includeGroups": [
      "String"
    ],
    "excludeGroups": [
      "String"
    ],
    "includeRoles": [
      "String"
    ],
    "excludeRoles": [
      "String"
    ]
  },
  "signInRiskLevels": [
    "String"
  ],
  "platforms": {
    "@odata.type": "microsoft.graph.conditionalAccessPlatforms",
    "includePlatforms": [
      "String"
    ],
    "excludePlatforms": [
      "String"
    ]
  },
  "locations": {
    "@odata.type": "microsoft.graph.conditionalAccessLocations",
    "includeLocations": [
      "String"
    ],
    "excludeLocations": [
      "String"
    ]
  },
  "clientAppTypes": [
    "String"
  ],
  "deviceStates": {
    "@odata.type": "microsoft.graph.conditionalAccessDeviceStates",
    "includeStates": [
      "String"
    ],
    "excludeStates": [
      "String"
    ]
  }
}
```

