---
title: "Get contactFolder"
description: "Read properties and relationships of the contactFolder object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get contactFolder

Namespace: microsoft.graph

Read properties and relationships of the [contactFolder](../resources/contactfolder.md) object.

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
GET /me/contactFolders/{contactFolderId}
GET /users/{usersId}/contactFolders/{contactFolderId}
GET /me/contactFolders/{contactFolderId}/childFolders/{contactFolderId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/contactFolders/{contactFolderId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 265

{
  "value": {
    "@odata.type": "#microsoft.graph.contactFolder",
    "id": "f4a2f5e4-f5e4-f4a2-e4f5-a2f4e4f5a2f4",
    "parentFolderId": "Parent Folder Id value",
    "displayName": "Display Name value",
    "wellKnownName": "Well Known Name value"
  }
}
```

