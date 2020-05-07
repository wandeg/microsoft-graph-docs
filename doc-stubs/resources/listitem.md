---
title: "listItem resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# listItem resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [baseItem](../resources/baseitem.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[getActivitiesByInterval](../api/listitem-getactivitiesbyinterval.md)|[itemActivityStat](../resources/itemactivitystat.md) collection|**TODO: Add Description**|
|[List createdByUser](../api/listitem-list-createdbyuser.md)|[user](../resources/user.md) collection|Get the users from the createdByUser navigation property.|
|[Add createdByUser](../api/listitem-post-createdbyuser.md)|[user](../resources/user.md)|Add createdByUser by posting to the createdByUser collection.|
|[Remove createdByUser](../api/listitem-delete-createdbyuser.md)|None|Remove a [user](../resources/user.md) object.|
|[List lastModifiedByUser](../api/listitem-list-lastmodifiedbyuser.md)|[user](../resources/user.md) collection|Get the users from the lastModifiedByUser navigation property.|
|[Add lastModifiedByUser](../api/listitem-post-lastmodifiedbyuser.md)|[user](../resources/user.md)|Add lastModifiedByUser by posting to the lastModifiedByUser collection.|
|[Remove lastModifiedByUser](../api/listitem-delete-lastmodifiedbyuser.md)|None|Remove a [user](../resources/user.md) object.|
|[List activities](../api/listitem-list-activities.md)|[itemActivityOLD](../resources/itemactivityold.md) collection|Get the itemActivityOLDs from the activities navigation property.|
|[Create activities](../api/listitem-post-activities.md)|[itemActivityOLD](../resources/itemactivityold.md)|Create a new activities object.|
|[Delete activities](../api/listitem-delete-activities.md)|None|Delete an [itemActivityOLD](../resources/itemactivityold.md) object.|
|[Update activities](../api/listitem-update-activities.md)|[itemActivityOLD](../resources/itemactivityold.md)|Update the properties of an activities object.|
|[Get itemActivityOLD](../api/itemactivityold-get.md)|[itemActivityOLD](../resources/itemactivityold.md)|Read the properties and relationships of an [itemActivityOLD](../resources/itemactivityold.md) object.|
|[List analytics](../api/listitem-list-analytics.md)|[itemAnalytics](../resources/itemanalytics.md) collection|Get the itemAnalytics from the analytics navigation property.|
|[Add analytics](../api/listitem-post-analytics.md)|[itemAnalytics](../resources/itemanalytics.md)|Add analytics by posting to the analytics collection.|
|[Remove analytics](../api/listitem-delete-analytics.md)|None|Remove an [itemAnalytics](../resources/itemanalytics.md) object.|
|[List driveItem](../api/listitem-list-driveitem.md)|[driveItem](../resources/driveitem.md) collection|Get the driveItems from the driveItem navigation property.|
|[Create driveItem](../api/listitem-post-driveitem.md)|[driveItem](../resources/driveitem.md)|Create a new driveItem object.|
|[Delete driveItem](../api/listitem-delete-driveitem.md)|None|Delete a [driveItem](../resources/driveitem.md) object.|
|[Update driveItem](../api/listitem-update-driveitem.md)|[driveItem](../resources/driveitem.md)|Update the properties of a driveItem object.|
|[Get driveItem](../api/driveitem-get.md)|[driveItem](../resources/driveitem.md)|Read the properties and relationships of a [driveItem](../resources/driveitem.md) object.|
|[List fields](../api/listitem-list-fields.md)|[fieldValueSet](../resources/fieldvalueset.md) collection|Get the fieldValueSets from the fields navigation property.|
|[Create fields](../api/listitem-post-fields.md)|[fieldValueSet](../resources/fieldvalueset.md)|Create a new fields object.|
|[Delete fields](../api/listitem-delete-fields.md)|None|Delete a [fieldValueSet](../resources/fieldvalueset.md) object.|
|[Update fields](../api/listitem-update-fields.md)|[fieldValueSet](../resources/fieldvalueset.md)|Update the properties of a fields object.|
|[Get fieldValueSet](../api/fieldvalueset-get.md)|[fieldValueSet](../resources/fieldvalueset.md)|Read the properties and relationships of a [fieldValueSet](../resources/fieldvalueset.md) object.|
|[List versions](../api/listitem-list-versions.md)|[listItemVersion](../resources/listitemversion.md) collection|Get the listItemVersions from the versions navigation property.|
|[Create versions](../api/listitem-post-versions.md)|[listItemVersion](../resources/listitemversion.md)|Create a new versions object.|
|[Delete versions](../api/listitem-delete-versions.md)|None|Delete a [listItemVersion](../resources/listitemversion.md) object.|
|[Update versions](../api/listitem-update-versions.md)|[listItemVersion](../resources/listitemversion.md)|Update the properties of a versions object.|
|[Get listItemVersion](../api/listitemversion-get.md)|[listItemVersion](../resources/listitemversion.md)|Read the properties and relationships of a [listItemVersion](../resources/listitemversion.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|contentType|[contentTypeInfo](../resources/contenttypeinfo.md)|**TODO: Add Description**|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|description|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|eTag|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|name|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|parentReference|[itemReference](../resources/itemreference.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|sharepointIds|[sharepointIds](../resources/sharepointids.md)|**TODO: Add Description**|
|webUrl|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|activities|[itemActivityOLD](../resources/itemactivityold.md) collection|**TODO: Add Description**|
|analytics|[itemAnalytics](../resources/itemanalytics.md)|**TODO: Add Description**|
|createdByUser|[user](../resources/user.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|driveItem|[driveItem](../resources/driveitem.md)|**TODO: Add Description**|
|fields|[fieldValueSet](../resources/fieldvalueset.md)|**TODO: Add Description**|
|lastModifiedByUser|[user](../resources/user.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|versions|[listItemVersion](../resources/listitemversion.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.itemReference"
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

