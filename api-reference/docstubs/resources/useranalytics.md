---
title: "userAnalytics resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userAnalytics resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userAnalytics](../api/useranalytics-get.md)|[userAnalytics](../resources/useranalytics.md)|Read the properties and relationships of a [userAnalytics](../resources/useranalytics.md) object.|
|[Update userAnalytics](../api/useranalytics-update.md)|[userAnalytics](../resources/useranalytics.md)|Update the properties of a [userAnalytics](../resources/useranalytics.md) object.|
|[List activityStatistics](../api/useranalytics-list-activitystatistics.md)|[activityStatistics](../resources/activitystatistics.md) collection|Get the activityStatistics from the activityStatistics navigation property.|
|[Create activityStatistics](../api/useranalytics-post-activitystatistics.md)|[activityStatistics](../resources/activitystatistics.md)|Create a new activityStatistics object.|
|[Delete activityStatistics](../api/useranalytics-delete-activitystatistics.md)|None|Delete an [activityStatistics](../resources/activitystatistics.md) object.|
|[Update activityStatistics](../api/useranalytics-update-activitystatistics.md)|[activityStatistics](../resources/activitystatistics.md)|Update the properties of an activityStatistics object.|
|[Get activityStatistics](../api/activitystatistics-get.md)|[activityStatistics](../resources/activitystatistics.md)|Read the properties and relationships of an [activityStatistics](../resources/activitystatistics.md) object.|
|[List analytics](../api/user-list-analytics.md)|[userAnalytics](../resources/useranalytics.md) collection|Get the userAnalytics from the analytics navigation property.|
|[Create analytics](../api/user-post-analytics.md)|[userAnalytics](../resources/useranalytics.md)|Create a new analytics object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|settings|[settings](../resources/settings.md)|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|activityStatistics|[activityStatistics](../resources/activitystatistics.md) collection|**TODO: Add Description**|

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

