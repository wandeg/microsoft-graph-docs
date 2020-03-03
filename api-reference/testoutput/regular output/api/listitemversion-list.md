---
title: "List listItemVersions"
description: "List properties and relationships of the listItemVersion objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List listItemVersions

Namespace: microsoft.graph

List properties and relationships of the [listItemVersion](../resources/listitemversion.md) objects.

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
GET /me/drive/items/{driveItemId}/listItem/versions
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [listItemVersion](../resources/listitemversion.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_listitemversion"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/listItem/versions
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.listitemversion)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 812

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.listItemVersion",
      "id": "f9c2983a-983a-f9c2-3a98-c2f93a98c2f9",
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
      "lastModifiedDateTime": "2017-01-01T00:00:08.5199759+03:00",
      "publication": {
        "@odata.type": "microsoft.graph.publicationFacet",
        "level": "Level value",
        "versionId": "Version Id value"
      }
    }
  ]
}
```

