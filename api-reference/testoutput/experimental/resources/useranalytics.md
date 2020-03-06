---
title: "userAnalytics resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userAnalytics resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userAnalytics](../api/useranalytics-get.md)|[userAnalytics](../resources/useranalytics.md)|Read properties and relationships of the [userAnalytics](../resources/useranalytics.md) object.|
|[Update userAnalytics](../api/useranalytics-update.md)|[userAnalytics](../resources/useranalytics.md)|Update the properties of a [userAnalytics](../resources/useranalytics.md) object.|
|[List activityStatistics](../api/useranalytics-list-activitystatistics.md)|[activityStatistics](../resources/activitystatistics.md) collection|Get the activityStatisticses from the activityStatistics navigation property.|
|[Add activityStatistics](../api/useranalytics-post-activitystatistics.md)|[activityStatistics](../resources/activitystatistics.md)|Add activityStatistics by posting to the activityStatistics collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|settings|[settings](../resources/settings.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|activityStatistics|[activityStatistics](../resources/activitystatistics.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userAnalytics",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userAnalytics",
  "id": "String (identifier)",
  "settings": {
    "@odata.type": "microsoft.graph.settings",
    "hasLicense": true,
    "hasOptedOut": true,
    "hasGraphMailbox": true
  }
}
```

