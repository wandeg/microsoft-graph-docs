---
title: "site resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# site resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [baseItem](../resources/baseitem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List sites](../api/site-list.md)|[site](../resources/site.md) collection|Get a list of the [site](../resources/site.md) objects and their properties.|
|[Get site](../api/site-get.md)|[site](../resources/site.md)|Read the properties and relationships of a [site](../resources/site.md) object.|
|[Create site](../api/site-post-sites.md)|[site](../resources/site.md)|Create a new [site](../resources/site.md) object.|
|[Delete site](../api/site-delete.md)|None|Deletes a [site](../resources/site.md) object.|
|[Update site](../api/site-update.md)|[site](../resources/site.md)|Update the properties of a [site](../resources/site.md) object.|
|[getActivitiesByInterval](../api/site-getactivitiesbyinterval.md)|[itemActivityStat](../resources/itemactivitystat.md) collection|**TODO: Add Description**|
|[getByPath](../api/site-getbypath.md)|[site](../resources/site.md)|**TODO: Add Description**|
|[add](../api/site-add.md)|[site](../resources/site.md) collection|**TODO: Add Description**|
|[remove](../api/site-remove.md)|[site](../resources/site.md) collection|**TODO: Add Description**|
|[List createdByUser](../api/site-list-createdbyuser.md)|[user](../resources/user.md) collection|Get the users from the createdByUser navigation property.|
|[Add createdByUser](../api/site-post-createdbyuser.md)|[user](../resources/user.md)|Add createdByUser by posting to the createdByUser collection.|
|[Remove createdByUser](../api/site-delete-createdbyuser.md)|None|Remove a [user](../resources/user.md) object.|
|[List lastModifiedByUser](../api/site-list-lastmodifiedbyuser.md)|[user](../resources/user.md) collection|Get the users from the lastModifiedByUser navigation property.|
|[Add lastModifiedByUser](../api/site-post-lastmodifiedbyuser.md)|[user](../resources/user.md)|Add lastModifiedByUser by posting to the lastModifiedByUser collection.|
|[Remove lastModifiedByUser](../api/site-delete-lastmodifiedbyuser.md)|None|Remove a [user](../resources/user.md) object.|
|[List analytics](../api/site-list-analytics.md)|[itemAnalytics](../resources/itemanalytics.md) collection|Get the itemAnalytics from the analytics navigation property.|
|[Add analytics](../api/site-post-analytics.md)|[itemAnalytics](../resources/itemanalytics.md)|Add analytics by posting to the analytics collection.|
|[Remove analytics](../api/site-delete-analytics.md)|None|Remove an [itemAnalytics](../resources/itemanalytics.md) object.|
|[List columns](../api/site-list-columns.md)|[columnDefinition](../resources/columndefinition.md) collection|Get the columnDefinitions from the columns navigation property.|
|[Create columns](../api/site-post-columns.md)|[columnDefinition](../resources/columndefinition.md)|Create a new columns object.|
|[Delete columns](../api/site-delete-columns.md)|None|Delete a [columnDefinition](../resources/columndefinition.md) object.|
|[Update columns](../api/site-update-columns.md)|[columnDefinition](../resources/columndefinition.md)|Update the properties of a columns object.|
|[Get columnDefinition](../api/columndefinition-get.md)|[columnDefinition](../resources/columndefinition.md)|Read the properties and relationships of a [columnDefinition](../resources/columndefinition.md) object.|
|[List contentTypes](../api/site-list-contenttypes.md)|[contentType](../resources/contenttype.md) collection|Get the contentTypes from the contentTypes navigation property.|
|[Create contentTypes](../api/site-post-contenttypes.md)|[contentType](../resources/contenttype.md)|Create a new contentTypes object.|
|[Delete contentTypes](../api/site-delete-contenttypes.md)|None|Delete a [contentType](../resources/contenttype.md) object.|
|[Update contentTypes](../api/site-update-contenttypes.md)|[contentType](../resources/contenttype.md)|Update the properties of a contentTypes object.|
|[Get contentType](../api/contenttype-get.md)|[contentType](../resources/contenttype.md)|Read the properties and relationships of a [contentType](../resources/contenttype.md) object.|
|[List drive](../api/site-list-drive.md)|[drive](../resources/drive.md) collection|Get the drives from the drive navigation property.|
|[Create drive](../api/site-post-drive.md)|[drive](../resources/drive.md)|Create a new drive object.|
|[Delete drive](../api/site-delete-drive.md)|None|Delete a [drive](../resources/drive.md) object.|
|[Update drive](../api/site-update-drive.md)|[drive](../resources/drive.md)|Update the properties of a drive object.|
|[Get drive](../api/drive-get.md)|[drive](../resources/drive.md)|Read the properties and relationships of a [drive](../resources/drive.md) object.|
|[List drives](../api/site-list-drives.md)|[drive](../resources/drive.md) collection|Get the drives from the drives navigation property.|
|[Create drives](../api/site-post-drives.md)|[drive](../resources/drive.md)|Create a new drives object.|
|[Delete drives](../api/site-delete-drives.md)|None|Delete a [drive](../resources/drive.md) object.|
|[Update drives](../api/site-update-drives.md)|[drive](../resources/drive.md)|Update the properties of a drives object.|
|[Get drive](../api/drive-get.md)|[drive](../resources/drive.md)|Read the properties and relationships of a [drive](../resources/drive.md) object.|
|[List items](../api/site-list-items.md)|[baseItem](../resources/baseitem.md) collection|Get the baseItems from the items navigation property.|
|[Create items](../api/site-post-items.md)|[baseItem](../resources/baseitem.md)|Create a new items object.|
|[Delete items](../api/site-delete-items.md)|None|Delete an [baseItem](../resources/baseitem.md) object.|
|[Update items](../api/site-update-items.md)|[baseItem](../resources/baseitem.md)|Update the properties of an items object.|
|[Get baseItem](../api/baseitem-get.md)|[baseItem](../resources/baseitem.md)|Read the properties and relationships of a [baseItem](../resources/baseitem.md) object.|
|[List lists](../api/site-list-lists.md)|[list](../resources/list.md) collection|Get the lists from the lists navigation property.|
|[Create lists](../api/site-post-lists.md)|[list](../resources/list.md)|Create a new lists object.|
|[Delete lists](../api/site-delete-lists.md)|None|Delete a [list](../resources/list.md) object.|
|[Update lists](../api/site-update-lists.md)|[list](../resources/list.md)|Update the properties of a lists object.|
|[Get list](../api/list-get.md)|[list](../resources/list.md)|Read the properties and relationships of a [list](../resources/list.md) object.|
|[List pages](../api/site-list-pages.md)|[sitePage](../resources/sitepage.md) collection|Get the sitePages from the pages navigation property.|
|[Create pages](../api/site-post-pages.md)|[sitePage](../resources/sitepage.md)|Create a new pages object.|
|[Delete pages](../api/site-delete-pages.md)|None|Delete a [sitePage](../resources/sitepage.md) object.|
|[Update pages](../api/site-update-pages.md)|[sitePage](../resources/sitepage.md)|Update the properties of a pages object.|
|[Get sitePage](../api/sitepage-get.md)|[sitePage](../resources/sitepage.md)|Read the properties and relationships of a [sitePage](../resources/sitepage.md) object.|
|[List sites](../api/site-list-sites.md)|[site](../resources/site.md) collection|Get the sites from the sites navigation property.|
|[Create sites](../api/site-post-sites.md)|[site](../resources/site.md)|Create a new sites object.|
|[Delete sites](../api/site-delete-sites.md)|None|Delete a [site](../resources/site.md) object.|
|[Update sites](../api/site-update-sites.md)|[site](../resources/site.md)|Update the properties of a sites object.|
|[Get site](../api/site-get.md)|[site](../resources/site.md)|Read the properties and relationships of a [site](../resources/site.md) object.|
|[List onenote](../api/site-list-onenote.md)|[onenote](../resources/onenote.md) collection|Get the onenotes from the onenote navigation property.|
|[Create onenote](../api/site-post-onenote.md)|[onenote](../resources/onenote.md)|Create a new onenote object.|
|[Delete onenote](../api/site-delete-onenote.md)|None|Delete an [onenote](../resources/onenote.md) object.|
|[Update onenote](../api/site-update-onenote.md)|[onenote](../resources/onenote.md)|Update the properties of an onenote object.|
|[Get onenote](../api/onenote-get.md)|[onenote](../resources/onenote.md)|Read the properties and relationships of an [onenote](../resources/onenote.md) object.|

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
|name|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|parentReference|[itemReference](../resources/itemreference.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|root|[root](../resources/root.md)|**TODO: Add Description**|
|sharepointIds|[sharepointIds](../resources/sharepointids.md)|**TODO: Add Description**|
|siteCollection|[siteCollection](../resources/sitecollection.md)|**TODO: Add Description**|
|webUrl|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|analytics|[itemAnalytics](../resources/itemanalytics.md)|**TODO: Add Description**|
|columns|[columnDefinition](../resources/columndefinition.md) collection|**TODO: Add Description**|
|contentTypes|[contentType](../resources/contenttype.md) collection|**TODO: Add Description**|
|createdByUser|[user](../resources/user.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|drive|[drive](../resources/drive.md)|**TODO: Add Description**|
|drives|[drive](../resources/drive.md) collection|**TODO: Add Description**|
|items|[baseItem](../resources/baseitem.md) collection|**TODO: Add Description**|
|lastModifiedByUser|[user](../resources/user.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|lists|[list](../resources/list.md) collection|**TODO: Add Description**|
|onenote|[onenote](../resources/onenote.md)|**TODO: Add Description**|
|pages|[sitePage](../resources/sitepage.md) collection|**TODO: Add Description**|
|sites|[site](../resources/site.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.site",
  "baseType": "microsoft.graph.baseItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.site",
  "id": "String (identifier)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
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
  "displayName": "String",
  "root": {
    "@odata.type": "microsoft.graph.root"
  },
  "sharepointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  },
  "siteCollection": {
    "@odata.type": "microsoft.graph.siteCollection",
    "dataLocationCode": "String",
    "hostname": "String"
  }
}
```

