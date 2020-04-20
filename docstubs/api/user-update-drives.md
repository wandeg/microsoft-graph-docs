---
title: "Update drives"
description: "Update the properties of a drives object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update drives

Namespace: microsoft.graph

Update the properties of a drives object.

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
PATCH /me/drives
PATCH /users/{usersId}/drives
PATCH /invitations/{invitationsId}/invitedUser/drives
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [drive](../resources/drive.md) object.

The following table shows the properties that are required when you create the [drive](../resources/drive.md).

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
|driveType|String|**TODO: Add Description**|
|owner|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|quota|[quota](../resources/quota.md)|**TODO: Add Description**|
|sharePointIds|[sharepointIds](../resources/sharepointids.md)|**TODO: Add Description**|
|system|[systemFacet](../resources/systemfacet.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [drive](../resources/drive.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_drives"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/drives
Content-Type: application/json
Content-length: 1696

{
  "@odata.type": "#microsoft.graph.drive",
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
  "driveType": "Drive Type value",
  "owner": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "quota": {
    "@odata.type": "microsoft.graph.quota",
    "deleted": 7,
    "remaining": 9,
    "state": "State value",
    "total": 5,
    "used": 4,
    "storagePlanInformation": {
      "@odata.type": "microsoft.graph.storagePlanInformation",
      "upgradeAvailable": true
    }
  },
  "sharePointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  },
  "system": {
    "@odata.type": "microsoft.graph.systemFacet"
  }
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.drive",
  "id": "0ed7ae38-ae38-0ed7-38ae-d70e38aed70e",
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
  "createdDateTime": "2016-12-31T23:57:02.5240758+03:00",
  "description": "Description value",
  "eTag": "ETag value",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "2017-01-01T00:01:44.3371159+03:00",
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
  "driveType": "Drive Type value",
  "owner": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "quota": {
    "@odata.type": "microsoft.graph.quota",
    "deleted": 7,
    "remaining": 9,
    "state": "State value",
    "total": 5,
    "used": 4,
    "storagePlanInformation": {
      "@odata.type": "microsoft.graph.storagePlanInformation",
      "upgradeAvailable": true
    }
  },
  "sharePointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  },
  "system": {
    "@odata.type": "microsoft.graph.systemFacet"
  }
}
```

