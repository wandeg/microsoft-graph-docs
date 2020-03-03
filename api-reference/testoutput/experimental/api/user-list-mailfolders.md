---
title: "List mailFolders"
description: "Get the mailFolders from the mailFolders navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List mailFolders

Namespace: microsoft.graph

Get the mailFolders from the mailFolders navigation property.

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
GET /me/mailFolders
GET /users/{usersId}/mailFolders
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [mailFolder](../resources/mailfolder.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/mailFolders
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.mailfolder)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 375

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mailFolder",
      "id": "f1deb285-b285-f1de-85b2-def185b2def1",
      "displayName": "Display Name value",
      "parentFolderId": "Parent Folder Id value",
      "childFolderCount": 0,
      "unreadItemCount": 15,
      "totalItemCount": 14,
      "wellKnownName": "Well Known Name value"
    }
  ]
}
```

