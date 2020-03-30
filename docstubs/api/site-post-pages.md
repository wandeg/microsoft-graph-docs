---
title: "Add pages"
description: "Add pages by posting to the pages collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add pages

Namespace: microsoft.graph

Add pages by posting to the pages collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /sites/{sitesId}/pages/$ref
POST /me/joinedGroups/{groupId}/sites/{siteId}/pages/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [sitePage](../resources/sitepage.md) object.

The following table shows the properties that are required when you create the [sitePage](../resources/sitepage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [baseItem](../resources/baseitem.md)|
|createdDateTime|DateTimeOffset| Inherited from [baseItem](../resources/baseitem.md)|
|description|String| Inherited from [baseItem](../resources/baseitem.md)|
|eTag|String| Inherited from [baseItem](../resources/baseitem.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [baseItem](../resources/baseitem.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [baseItem](../resources/baseitem.md)|
|name|String| Inherited from [baseItem](../resources/baseitem.md)|
|parentReference|[itemReference](../resources/itemreference.md)| Inherited from [baseItem](../resources/baseitem.md)|
|webUrl|String| Inherited from [baseItem](../resources/baseitem.md)|
|title|String||
|contentType|[contentTypeInfo](../resources/contenttypeinfo.md)||
|pageLayoutType|String||
|webParts|[webPart](../resources/webpart.md) collection||
|publishingState|[publicationFacet](../resources/publicationfacet.md)||



## Response
If successful, this method returns a `201 Created` response code and a [sitePage](../resources/sitepage.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_sitepage_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/sites/{sitesId}/pages
Content-type: application/json
Content-length: 1641

{
  "@odata.type": "#microsoft.graph.sitePage",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "description": "Description value",
  "eTag": "ETag value",
  "name": "Name value",
  "parentReference": {
    "@odata.type": "microsoft.graph.itemReference",
    "driveId": "Drive Id value",
    "driveType": "Drive Type value",
    "path": "Path value",
    "shareId": "Share Id value",
    "sharepointIds": {
      "@odata.type": "microsoft.graph.sharepointIds",
      "listId": "List Id value",
      "listItemId": "List Item Id value",
      "listItemUniqueId": "List Item Unique Id value",
      "siteId": "Site Id value",
      "siteUrl": "https://example.com/siteUrl/",
      "tenantId": "Tenant Id value",
      "webId": "Web Id value"
    }
  },
  "webUrl": "https://example.com/webUrl/",
  "title": "Title value",
  "contentType": {
    "@odata.type": "microsoft.graph.contentTypeInfo"
  },
  "pageLayoutType": "Page Layout Type value",
  "webParts": [
    {
      "@odata.type": "microsoft.graph.webPart",
      "type": "Type value",
      "data": {
        "@odata.type": "microsoft.graph.sitePageData"
      }
    }
  ],
  "publishingState": {
    "@odata.type": "microsoft.graph.publicationFacet",
    "level": "Level value",
    "versionId": "Version Id value"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sitepage"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1892

{
  "@odata.type": "#microsoft.graph.sitePage",
  "id": "961239af-39af-9612-af39-1296af391296",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
  "description": "Description value",
  "eTag": "ETag value",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
  "name": "Name value",
  "parentReference": {
    "@odata.type": "microsoft.graph.itemReference",
    "driveId": "Drive Id value",
    "driveType": "Drive Type value",
    "path": "Path value",
    "shareId": "Share Id value",
    "sharepointIds": {
      "@odata.type": "microsoft.graph.sharepointIds",
      "listId": "List Id value",
      "listItemId": "List Item Id value",
      "listItemUniqueId": "List Item Unique Id value",
      "siteId": "Site Id value",
      "siteUrl": "https://example.com/siteUrl/",
      "tenantId": "Tenant Id value",
      "webId": "Web Id value"
    }
  },
  "webUrl": "https://example.com/webUrl/",
  "title": "Title value",
  "contentType": {
    "@odata.type": "microsoft.graph.contentTypeInfo"
  },
  "pageLayoutType": "Page Layout Type value",
  "webParts": [
    {
      "@odata.type": "microsoft.graph.webPart",
      "type": "Type value",
      "data": {
        "@odata.type": "microsoft.graph.sitePageData"
      }
    }
  ],
  "publishingState": {
    "@odata.type": "microsoft.graph.publicationFacet",
    "level": "Level value",
    "versionId": "Version Id value"
  }
}
```

