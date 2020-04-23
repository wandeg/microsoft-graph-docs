---
title: "Get listItemVersion"
description: "Read the properties and relationships of a listItemVersion object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get listItemVersion

Namespace: microsoft.graph

Read the properties and relationships of a [listItemVersion](../resources/listitemversion.md) object.

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
GET /invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/listItem/versions/{listItemVersionId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [listItemVersion](../resources/listitemversion.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_listitemversion"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/listItem/versions/{listItemVersionId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.listItemVersion"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.listItemVersion",
    "id": "a7b0cb2a-cb2a-a7b0-2acb-b0a72acbb0a7",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet",
      "application": {
        "@odata.type": "microsoft.graph.identity",
        "displayName": "Display Name value",
        "id": "Id value"
      },
      "device": {
        "@odata.type": "microsoft.graph.identity"
      },
      "user": {
        "@odata.type": "microsoft.graph.identity"
      }
    },
    "lastModifiedDateTime": "2017-01-01T00:02:46.687785+03:00",
    "publication": {
      "@odata.type": "microsoft.graph.publicationFacet",
      "level": "Level value",
      "versionId": "Version Id value"
    }
  }
}
```

