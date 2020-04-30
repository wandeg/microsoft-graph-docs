---
title: "Update roleManagement"
description: "Update the properties of a roleManagement object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update roleManagement

Namespace: Microsoft.DirectoryServices

Update the properties of a [roleManagement](../resources/microsoft.directoryservices-rolemanagement.md) object.

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
PATCH /roleManagement
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [roleManagement](../resources/microsoft.directoryservices-rolemanagement.md) object.

The following table shows the properties that are required when you create the [roleManagement](../resources/microsoft.directoryservices-rolemanagement.md).

|Property|Type|Description|
|:---|:---|:---|



## Response
If successful, this method returns a `200 OK` response code and an updated [roleManagement](../resources/microsoft.directoryservices-rolemanagement.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_rolemanagement"
}
-->
``` http
PATCH https://graph.microsoft.com/changelog/roleManagement
Content-Type: application/json
Content-length: 68

{
  "@odata.type": "#Microsoft.DirectoryServices.roleManagement"
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
  "@odata.type": "#Microsoft.DirectoryServices.roleManagement"
}
```

