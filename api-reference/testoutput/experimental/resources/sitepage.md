---
title: "sitePage resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# sitePage resource type




Inherits from [baseItem](../resources/baseItem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get sitePage](../api/sitepage-get.md)|[sitePage](../resources/sitePage.md)|Read properties and relationships of the [sitePage](../resources/sitepage.md) object.|
|[Delete sitePage](../api/sitepage-delete.md)|None|Deletes a [sitePage](../resources/sitepage.md).|
|[Update sitePage](../api/sitepage-update.md)|[sitePage](../resources/sitePage.md)|Update the properties of a [sitePage](../resources/sitepage.md) object.|
|[publish](../api/sitepage-publish.md)|None||
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|

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
|pageLayoutType|String||
|parentReference|[itemReference](../resources/itemReference.md)| Inherited from [baseItem](../resources/baseItem.md)|
|publishingState|[publicationFacet](../resources/publicationFacet.md)||
|title|String||
|webParts|[webPart](../resources/webPart.md) collection||
|webUrl|String| Inherited from [baseItem](../resources/baseItem.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|createdByUser|[user](../resources/user.md)| Inherited from [baseItem](../resources/baseItem.md)|
|lastModifiedByUser|[user](../resources/user.md)| Inherited from [baseItem](../resources/baseItem.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sitePage",
  "baseType": "microsoft.graph.baseItem",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sitePage",
  "id": "String (identifier)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String"
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
  "title": "String",
  "contentType": {
    "@odata.type": "microsoft.graph.contentTypeInfo"
  },
  "pageLayoutType": "String",
  "webParts": [
    {
      "@odata.type": "microsoft.graph.webPart",
      "type": "String",
      "data": {
        "@odata.type": "microsoft.graph.sitePageData"
      }
    }
  ],
  "publishingState": {
    "@odata.type": "microsoft.graph.publicationFacet",
    "level": "String",
    "versionId": "String"
  }
}
```

