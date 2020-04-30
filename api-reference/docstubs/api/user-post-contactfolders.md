---
title: "Create contactFolders"
description: "Create a new contactFolders object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create contactFolders

Namespace: microsoft.graph

Create a new contactFolders object.

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
POST /me/contactFolders
POST /users/{usersId}/contactFolders
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [contactFolder](../resources/contactfolder.md) object.

The following table shows the properties that are required when you create the [contactFolder](../resources/contactfolder.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|parentFolderId|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|wellKnownName|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [contactFolder](../resources/contactfolder.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/contactFolders
Content-Type: application/json
Content-length: 144

{
  "@odata.type": "#microsoft.graph.contactFolder",
  "parentFolderId": "String",
  "displayName": "String",
  "wellKnownName": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactfolder"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.contactFolder",
  "id": "ad2075a3-75a3-ad20-a375-20ada37520ad",
  "parentFolderId": "String",
  "displayName": "String",
  "wellKnownName": "String"
}
```

