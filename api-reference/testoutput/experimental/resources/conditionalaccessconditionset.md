---
title: "conditionalAccessConditionSet resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# conditionalAccessConditionSet resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|applications|[conditionalAccessApplications](../resources/conditionalAccessApplications.md)||
|clientAppTypes|Enumeration collection||
|deviceStates|[conditionalAccessDeviceStates](../resources/conditionalAccessDeviceStates.md)||
|locations|[conditionalAccessLocations](../resources/conditionalAccessLocations.md)||
|platforms|[conditionalAccessPlatforms](../resources/conditionalAccessPlatforms.md)||
|signInRiskLevels|Enumeration collection||
|users|[conditionalAccessUsers](../resources/conditionalAccessUsers.md)||

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

