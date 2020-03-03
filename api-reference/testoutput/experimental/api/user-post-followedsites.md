---
title: "Create followedSites"
description: "Create followedSites by posting to the followedSites collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create followedSites

Create followedSites by posting to the followedSites collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/followedSites/$ref
POST /users/{usersId}/followedSites/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the site object.

The following table shows the properties that are required when you create the site.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdBy|[identitySet](../resources/identitySet.md)| Inherited from [baseItem](../resources/baseItem.md)|
|createdDateTime|DateTimeOffset| Inherited from [baseItem](../resources/baseItem.md)|
|description|String| Inherited from [baseItem](../resources/baseItem.md)|
|eTag|String| Inherited from [baseItem](../resources/baseItem.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [baseItem](../resources/baseItem.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [baseItem](../resources/baseItem.md)|
|name|String| Inherited from [baseItem](../resources/baseItem.md)|
|parentReference|[itemReference](../resources/itemReference.md)| Inherited from [baseItem](../resources/baseItem.md)|
|webUrl|String| Inherited from [baseItem](../resources/baseItem.md)|
|displayName|String||
|root|[root](../resources/root.md)||
|sharepointIds|[sharepointIds](../resources/sharepointIds.md)||
|siteCollection|[siteCollection](../resources/siteCollection.md)||



## Response
If successful, this method returns a `201 Created` response code and a [site](../resources/site.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_site_from_sites"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/me/followedSites
Content-type: application/json
Content-length: 1487

{
  "@odata.type": "#microsoft.graph.site",
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
  "displayName": "Display Name value",
  "root": {
    "@odata.type": "microsoft.graph.root"
  },
  "sharepointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  },
  "siteCollection": {
    "@odata.type": "microsoft.graph.siteCollection",
    "dataLocationCode": "Data Location Code value",
    "hostname": "Hostname value"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.site"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1738

{
  "@odata.type": "#microsoft.graph.site",
  "id": "5c359121-9121-5c35-2191-355c2191355c",
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
  "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
  "description": "Description value",
  "eTag": "ETag value",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
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
  "displayName": "Display Name value",
  "root": {
    "@odata.type": "microsoft.graph.root"
  },
  "sharepointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  },
  "siteCollection": {
    "@odata.type": "microsoft.graph.siteCollection",
    "dataLocationCode": "Data Location Code value",
    "hostname": "Hostname value"
  }
}
```

