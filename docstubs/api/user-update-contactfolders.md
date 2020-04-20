---
title: "Update contactFolders"
description: "Update the properties of a contactFolders object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update contactFolders

Namespace: microsoft.graph

Update the properties of a contactFolders object.

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
PATCH /me/contactFolders
PATCH /users/{usersId}/contactFolders
PATCH /invitations/{invitationsId}/invitedUser/contactFolders
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [contactFolder](../resources/contactfolder.md) object.

The following table shows the properties that are required when you create the [contactFolder](../resources/contactfolder.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|parentFolderId|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|wellKnownName|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [contactFolder](../resources/contactfolder.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_contactfolders"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/contactFolders
Content-Type: application/json
Content-length: 187

{
  "@odata.type": "#microsoft.graph.contactFolder",
  "parentFolderId": "Parent Folder Id value",
  "displayName": "Display Name value",
  "wellKnownName": "Well Known Name value"
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
  "@odata.type": "#microsoft.graph.contactFolder",
  "id": "c7d098a9-98a9-c7d0-a998-d0c7a998d0c7",
  "parentFolderId": "Parent Folder Id value",
  "displayName": "Display Name value",
  "wellKnownName": "Well Known Name value"
}
```

