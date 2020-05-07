---
title: "Update operations"
description: "Update the properties of an operations object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update operations

Namespace: microsoft.graph

Update the properties of an operations object.

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
PATCH /users/{usersId}/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [managedAppOperation](../resources/managedappoperation.md) object.

The following table shows the properties that are required when you create the [managedAppOperation](../resources/managedappoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|state|String|**TODO: Add Description**|
|version|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/managedappoperation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_operations"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/managedAppRegistrations/{managedAppRegistrationId}/operations
Content-Type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "String",
  "state": "String",
  "version": "String"
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
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "id": "b88a7d49-7d49-b88a-497d-8ab8497d8ab8",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "version": "String"
}
```

