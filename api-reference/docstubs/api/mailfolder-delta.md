---
title: "mailFolder: delta"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# delta

Namespace: microsoft.graph

**TODO: Add Description**

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
GET /me/mailFolders/delta
GET /users/{usersId}/mailFolders/delta
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [mailFolder](../resources/mailfolder.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "mailfolder_delta"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/mailFolders/delta
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.mailfolder)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mailFolder",
      "id": "cde6ba08-ba08-cde6-08ba-e6cd08bae6cd",
      "displayName": "Display Name value",
      "parentFolderId": "Parent Folder Id value",
      "childFolderCount": 0,
      "unreadItemCount": 15,
      "totalItemCount": 14
    }
  ]
}
```

