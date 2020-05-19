---
title: "list resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# list resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [baseItem](../resources/baseitem.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List list](../api/drive-list-list.md)|[list](../resources/list.md) collection|Get the lists from the list navigation property.|
|[Create list](../api/drive-post-list.md)|[list](../resources/list.md)|Create a new list object.|
|[Delete list](../api/drive-delete-list.md)|None|Delete a [list](../resources/list.md) object.|
|[Update list](../api/drive-update-list.md)|[list](../resources/list.md)|Update the properties of a list object.|
|[Get list](../api/drive-get-list.md)|[list](../resources/list.md)|Read the properties and relationships of a [list](../resources/list.md) object.|
|[List createdByUser](../api/list-list-createdbyuser.md)|[user](../resources/user.md) collection|Get the users from the createdByUser navigation property.|
|[Add createdByUser](../api/list-post-createdbyuser.md)|[user](../resources/user.md)|Add createdByUser by posting to the createdByUser collection.|
|[Remove createdByUser](../api/list-delete-createdbyuser.md)|None|Remove a [user](../resources/user.md) object.|
|[List lastModifiedByUser](../api/list-list-lastmodifiedbyuser.md)|[user](../resources/user.md) collection|Get the users from the lastModifiedByUser navigation property.|
|[Add lastModifiedByUser](../api/list-post-lastmodifiedbyuser.md)|[user](../resources/user.md)|Add lastModifiedByUser by posting to the lastModifiedByUser collection.|
|[Remove lastModifiedByUser](../api/list-delete-lastmodifiedbyuser.md)|None|Remove a [user](../resources/user.md) object.|
|[List columns](../api/list-list-columns.md)|[columnDefinition](../resources/columndefinition.md) collection|Get the columnDefinitions from the columns navigation property.|
|[Create columns](../api/list-post-columns.md)|[columnDefinition](../resources/columndefinition.md)|Create a new columns object.|
|[Delete columns](../api/list-delete-columns.md)|None|Delete a [columnDefinition](../resources/columndefinition.md) object.|
|[Update columns](../api/list-update-columns.md)|[columnDefinition](../resources/columndefinition.md)|Update the properties of a columns object.|
|[Get columns](../api/list-get-columndefinition.md)|[columnDefinition](../resources/columndefinition.md)|Read the properties and relationships of a [columnDefinition](../resources/columndefinition.md) object.|
|[List contentTypes](../api/list-list-contenttypes.md)|[contentType](../resources/contenttype.md) collection|Get the contentTypes from the contentTypes navigation property.|
|[Create contentTypes](../api/list-post-contenttypes.md)|[contentType](../resources/contenttype.md)|Create a new contentTypes object.|
|[Delete contentTypes](../api/list-delete-contenttypes.md)|None|Delete a [contentType](../resources/contenttype.md) object.|
|[Update contentTypes](../api/list-update-contenttypes.md)|[contentType](../resources/contenttype.md)|Update the properties of a contentTypes object.|
|[Get contentTypes](../api/list-get-contenttype.md)|[contentType](../resources/contenttype.md)|Read the properties and relationships of a [contentType](../resources/contenttype.md) object.|
|[List drive](../api/list-list-drive.md)|[drive](../resources/drive.md) collection|Get the drives from the drive navigation property.|
|[Create drive](../api/list-post-drive.md)|[drive](../resources/drive.md)|Create a new drive object.|
|[Delete drive](../api/list-delete-drive.md)|None|Delete a [drive](../resources/drive.md) object.|
|[Update drive](../api/list-update-drive.md)|[drive](../resources/drive.md)|Update the properties of a drive object.|
|[Get drive](../api/list-get-drive.md)|[drive](../resources/drive.md)|Read the properties and relationships of a [drive](../resources/drive.md) object.|
|[List items](../api/list-list-items.md)|[listItem](../resources/listitem.md) collection|Get the listItems from the items navigation property.|
|[Create items](../api/list-post-items.md)|[listItem](../resources/listitem.md)|Create a new items object.|
|[Delete items](../api/list-delete-items.md)|None|Delete a [listItem](../resources/listitem.md) object.|
|[Update items](../api/list-update-items.md)|[listItem](../resources/listitem.md)|Update the properties of an items object.|
|[Get items](../api/list-get-listitem.md)|[listItem](../resources/listitem.md)|Read the properties and relationships of a [listItem](../resources/listitem.md) object.|
|[List subscriptions](../api/list-list-subscriptions.md)|[subscription](../resources/subscription.md) collection|Get the subscriptions from the subscriptions navigation property.|
|[Create subscriptions](../api/list-post-subscriptions.md)|[subscription](../resources/subscription.md)|Create a new subscriptions object.|
|[Delete subscriptions](../api/list-delete-subscriptions.md)|None|Delete a [subscription](../resources/subscription.md) object.|
|[Update subscriptions](../api/list-update-subscriptions.md)|[subscription](../resources/subscription.md)|Update the properties of a subscriptions object.|
|[Get subscriptions](../api/list-get-subscription.md)|[subscription](../resources/subscription.md)|Read the properties and relationships of a [subscription](../resources/subscription.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|description|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|displayName|String|**TODO: Add Description**|
|eTag|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|list|[listInfo](../resources/listinfo.md)|**TODO: Add Description**|
|name|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|parentReference|[itemReference](../resources/itemreference.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|sharepointIds|[sharepointIds](../resources/sharepointids.md)|**TODO: Add Description**|
|system|[systemFacet](../resources/systemfacet.md)|**TODO: Add Description**|
|webUrl|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|columns|[columnDefinition](../resources/columndefinition.md) collection|**TODO: Add Description**|
|contentTypes|[contentType](../resources/contenttype.md) collection|**TODO: Add Description**|
|createdByUser|[user](../resources/user.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|drive|[drive](../resources/drive.md)|**TODO: Add Description**|
|items|[listItem](../resources/listitem.md) collection|**TODO: Add Description**|
|lastModifiedByUser|[user](../resources/user.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|subscriptions|[subscription](../resources/subscription.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.list",
  "baseType": "microsoft.graph.baseItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.list",
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
  "displayName": "String",
  "list": {
    "@odata.type": "microsoft.graph.listInfo"
  },
  "sharepointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  },
  "system": {
    "@odata.type": "microsoft.graph.systemFacet"
  }
}
```

