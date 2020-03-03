---
title: "userAnalytics resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# userAnalytics resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List userAnalyticses](../api/useranalytics-list.md)|[userAnalytics](../resources/userAnalytics.md) collection|List properties and relationships of the [userAnalytics](../resources/useranalytics.md) objects.|
|[Get userAnalytics](../api/useranalytics-get.md)|[userAnalytics](../resources/userAnalytics.md)|Read properties and relationships of the [userAnalytics](../resources/useranalytics.md) object.|
|[Create userAnalytics](../api/useranalytics-create.md)|[userAnalytics](../resources/userAnalytics.md)|Create a new [userAnalytics](../resources/useranalytics.md) object.|
|[Delete userAnalytics](../api/useranalytics-delete.md)|None|Deletes a [userAnalytics](../resources/useranalytics.md).|
|[Update userAnalytics](../api/useranalytics-update.md)|[userAnalytics](../resources/userAnalytics.md)|Update the properties of a [userAnalytics](../resources/useranalytics.md) object.|
|[List activityStatistics](../api/useranalytics-list-activitystatistics.md)|[activityStatistics](../resources/activityStatistics.md) collection|Get the activityStatisticses from the activityStatistics navigation property.|
|[Add activityStatistics](../api/useranalytics-post-activitystatistics.md)|[activityStatistics](../resources/activityStatistics.md)|Add activityStatistics by posting to the activityStatistics collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|settings|[settings](../resources/settings.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|activityStatistics|[activityStatistics](../resources/activityStatistics.md) collection||

## JSON Representation
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

