---
title: "Create mailFolders"
description: "Create a new mailFolders object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create mailFolders

Namespace: microsoft.graph

Create a new mailFolders object.

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
POST /me/mailFolders
POST /users/{usersId}/mailFolders
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [mailFolder](../resources/mailfolder.md) object.

The following table shows the properties that are required when you create the [mailFolder](../resources/mailfolder.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|parentFolderId|String|**TODO: Add Description**|
|childFolderCount|Int32|**TODO: Add Description**|
|unreadItemCount|Int32|**TODO: Add Description**|
|totalItemCount|Int32|**TODO: Add Description**|
|wellKnownName|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/mailFolders
Content-Type: application/json
Content-length: 261

{
  "@odata.type": "#microsoft.graph.mailFolder",
  "displayName": "Display Name value",
  "parentFolderId": "Parent Folder Id value",
  "childFolderCount": 0,
  "unreadItemCount": 15,
  "totalItemCount": 14,
  "wellKnownName": "Well Known Name value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailfolder"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.mailFolder",
  "id": "cf89f8c5-f8c5-cf89-c5f8-89cfc5f889cf",
  "displayName": "Display Name value",
  "parentFolderId": "Parent Folder Id value",
  "childFolderCount": 0,
  "unreadItemCount": 15,
  "totalItemCount": 14,
  "wellKnownName": "Well Known Name value"
}
```

