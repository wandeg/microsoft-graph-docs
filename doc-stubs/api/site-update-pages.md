---
title: "Update pages"
description: "Update the properties of a pages object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update pages

Namespace: microsoft.graph

Update the properties of a pages object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /sites/{sitesId}/pages
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [sitePage](../resources/sitepage.md) object.

The following table shows the properties that are required when you create the [sitePage](../resources/sitepage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|description|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|eTag|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|name|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|parentReference|[itemReference](../resources/itemreference.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|webUrl|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|title|String|**TODO: Add Description**|
|contentType|[contentTypeInfo](../resources/contenttypeinfo.md)|**TODO: Add Description**|
|pageLayoutType|String|**TODO: Add Description**|
|webParts|[webPart](../resources/webpart.md) collection|**TODO: Add Description**|
|publishingState|[publicationFacet](../resources/publicationfacet.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [sitePage](../resources/sitepage.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_pages"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/sites/{sitesId}/pages
Content-Type: application/json
Content-length: 602

{
  "@odata.type": "#microsoft.graph.sitePage",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "description": "String",
  "eTag": "String",
  "name": "String",
  "parentReference": {
    "@odata.type": "microsoft.graph.itemReference"
  },
  "webUrl": "String",
  "title": "String",
  "contentType": {
    "@odata.type": "microsoft.graph.contentTypeInfo"
  },
  "pageLayoutType": "String",
  "webParts": [
    {
      "@odata.type": "microsoft.graph.webPart"
    }
  ],
  "publishingState": {
    "@odata.type": "microsoft.graph.publicationFacet"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.sitePage",
  "id": "2699048d-048d-2699-8d04-99268d049926",
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
  "title": "String",
  "contentType": {
    "@odata.type": "microsoft.graph.contentTypeInfo"
  },
  "pageLayoutType": "String",
  "webParts": [
    {
      "@odata.type": "microsoft.graph.webPart"
    }
  ],
  "publishingState": {
    "@odata.type": "microsoft.graph.publicationFacet"
  }
}
```

