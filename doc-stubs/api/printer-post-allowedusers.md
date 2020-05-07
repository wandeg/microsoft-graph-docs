---
title: "Create allowedUsers"
description: "Create a new allowedUsers object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create allowedUsers

Namespace: microsoft.graph

Create a new allowedUsers object.

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
POST /print/printers/{printerId}/allowedUsers
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [printUserIdentity](../resources/printuseridentity.md) object.

The following table shows the properties that are required when you create the [printUserIdentity](../resources/printuseridentity.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|ipAddress|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [printUserIdentity](../resources/printuseridentity.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_printuseridentity_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/print/printers/{printerId}/allowedUsers
Content-Type: application/json
Content-length: 147

{
  "@odata.type": "#microsoft.graph.printUserIdentity",
  "displayName": "String",
  "ipAddress": "String",
  "userPrincipalName": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printuseridentity"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.printUserIdentity",
  "id": "18c3a06d-a06d-18c3-6da0-c3186da0c318",
  "displayName": "String",
  "ipAddress": "String",
  "userPrincipalName": "String"
}
```

