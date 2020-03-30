---
title: "Update contactFolder"
description: "Update the properties of a contactFolder object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update contactFolder

Namespace: microsoft.graph

Update the properties of a [contactFolder](../resources/contactfolder.md) object.

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
PATCH /me/contactFolders/{contactFolderId}
PATCH /users/{usersId}/contactFolders/{contactFolderId}
PATCH /me/contactFolders/{contactFolderId}/childFolders/{contactFolderId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [contactFolder](../resources/contactfolder.md) object.

The following table shows the properties that are required when you create the [contactFolder](../resources/contactfolder.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|parentFolderId|String||
|displayName|String||
|wellKnownName|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [contactFolder](../resources/contactfolder.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/contactFolders/{contactFolderId}
Content-type: application/json
Content-length: 187

{
  "@odata.type": "#microsoft.graph.contactFolder",
  "parentFolderId": "Parent Folder Id value",
  "displayName": "Display Name value",
  "wellKnownName": "Well Known Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 236

{
  "@odata.type": "#microsoft.graph.contactFolder",
  "id": "24ea3e19-3e19-24ea-193e-ea24193eea24",
  "parentFolderId": "Parent Folder Id value",
  "displayName": "Display Name value",
  "wellKnownName": "Well Known Name value"
}
```

