---
title: "conditionalAccessConditionSet resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# conditionalAccessConditionSet resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applications|[conditionalAccessApplications](../resources/conditionalaccessapplications.md)|**TODO: Add Description**|
|clientAppTypes|conditionalAccessClientApp collection|**TODO: Add Description**|
|devices|[conditionalAccessDevices](../resources/conditionalaccessdevices.md)|**TODO: Add Description**|
|deviceStates|[conditionalAccessDeviceStates](../resources/conditionalaccessdevicestates.md)|**TODO: Add Description**|
|locations|[conditionalAccessLocations](../resources/conditionalaccesslocations.md)|**TODO: Add Description**|
|platforms|[conditionalAccessPlatforms](../resources/conditionalaccessplatforms.md)|**TODO: Add Description**|
|signInRiskLevels|riskLevel collection|**TODO: Add Description**|
|users|[conditionalAccessUsers](../resources/conditionalaccessusers.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
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
  },
  "devices": {
    "@odata.type": "microsoft.graph.conditionalAccessDevices",
    "includeDeviceStates": [
      "String"
    ],
    "excludeDeviceStates": [
      "String"
    ]
  }
}
```

