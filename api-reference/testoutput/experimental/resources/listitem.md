---
title: "listItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# listItem resource type




Inherits from [baseItem](../resources/baseItem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get listItem](../api/listitem-get.md)|[listItem](../resources/listItem.md)|Read properties and relationships of the [listItem](../resources/listitem.md) object.|
|[Delete listItem](../api/listitem-delete.md)|None|Deletes a [listItem](../resources/listitem.md).|
|[Update listItem](../api/listitem-update.md)|[listItem](../resources/listItem.md)|Update the properties of a [listItem](../resources/listitem.md) object.|
|[getActivitiesByInterval](../api/listitem-getactivitiesbyinterval.md)|[itemActivityStat](../resources/itemActivityStat.md) collection||
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|
|[List activities](../api/listitem-list-activities.md)|[itemActivityOLD](../resources/itemActivityOLD.md) collection|Get the itemActivityOLDs from the activities navigation property.|
|[Add activities](../api/listitem-post-activities.md)|[itemActivityOLD](../resources/itemActivityOLD.md)|Add activities by posting to the activities collection.|
|[Get itemAnalytics](../api/itemanalytics-get.md)|[itemAnalytics](../resources/itemAnalytics.md)|Read properties and relationships of the [itemAnalytics](../resources/itemanalytics.md) object.|
|[Get driveItem](../api/driveitem-get.md)|[driveItem](../resources/driveItem.md)|Read properties and relationships of the [driveItem](../resources/driveitem.md) object.|
|[Get fieldValueSet](../api/fieldvalueset-get.md)|[fieldValueSet](../resources/fieldValueSet.md)|Read properties and relationships of the [fieldValueSet](../resources/fieldvalueset.md) object.|
|[List versions](../api/listitem-list-versions.md)|[listItemVersion](../resources/listItemVersion.md) collection|Get the listItemVersions from the versions navigation property.|
|[Add versions](../api/listitem-post-versions.md)|[listItemVersion](../resources/listItemVersion.md)|Add versions by posting to the versions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|contentType|[contentTypeInfo](../resources/contentTypeInfo.md)||
|createdBy|[identitySet](../resources/identitySet.md)| Inherited from [baseItem](../resources/baseItem.md)|
|createdDateTime|DateTimeOffset| Inherited from [baseItem](../resources/baseItem.md)|
|description|String| Inherited from [baseItem](../resources/baseItem.md)|
|eTag|String| Inherited from [baseItem](../resources/baseItem.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [baseItem](../resources/baseItem.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [baseItem](../resources/baseItem.md)|
|name|String| Inherited from [baseItem](../resources/baseItem.md)|
|parentReference|[itemReference](../resources/itemReference.md)| Inherited from [baseItem](../resources/baseItem.md)|
|sharepointIds|[sharepointIds](../resources/sharepointIds.md)||
|webUrl|String| Inherited from [baseItem](../resources/baseItem.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|activities|[itemActivityOLD](../resources/itemActivityOLD.md) collection||
|analytics|[itemAnalytics](../resources/itemAnalytics.md)||
|createdByUser|[user](../resources/user.md)| Inherited from [baseItem](../resources/baseItem.md)|
|driveItem|[driveItem](../resources/driveItem.md)||
|fields|[fieldValueSet](../resources/fieldValueSet.md)||
|lastModifiedByUser|[user](../resources/user.md)| Inherited from [baseItem](../resources/baseItem.md)|
|versions|[listItemVersion](../resources/listItemVersion.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.listItem",
  "baseType": "microsoft.graph.baseItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.listItem",
  "id": "String (identifier)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "eTag": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "name": "String",
  "parentReference": {
    "@odata.type": "microsoft.graph.itemReference",
    "driveId": "String",
    "driveType": "String",
    "path": "String",
    "shareId": "String",
    "sharepointIds": {
      "@odata.type": "microsoft.graph.sharepointIds",
      "listId": "String",
      "listItemId": "String",
      "listItemUniqueId": "String",
      "siteId": "String",
      "siteUrl": "String",
      "tenantId": "String",
      "webId": "String"
    }
  },
  "webUrl": "String",
  "contentType": {
    "@odata.type": "microsoft.graph.contentTypeInfo"
  },
  "sharepointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  }
}
```

