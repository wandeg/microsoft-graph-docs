---
title: "Update allowedUsers"
description: "Update the properties of an allowedUsers object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update allowedUsers

Namespace: microsoft.graph

Update the properties of an allowedUsers object.

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
PATCH /print/printers/{printerId}/allowedUsers
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
If successful, this method returns a `200 OK` response code and an updated [printUserIdentity](../resources/printuseridentity.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_allowedusers"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/print/printers/{printerId}/allowedUsers
Content-Type: application/json
Content-length: 188

{
  "@odata.type": "#microsoft.graph.printUserIdentity",
  "displayName": "Display Name value",
  "ipAddress": "Ip Address value",
  "userPrincipalName": "User Principal Name value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.printUserIdentity",
  "id": "2307d78a-d78a-2307-8ad7-07238ad70723",
  "displayName": "Display Name value",
  "ipAddress": "Ip Address value",
  "userPrincipalName": "User Principal Name value"
}
```

