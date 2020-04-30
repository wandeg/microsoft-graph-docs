---
title: "Update rbacApplication"
description: "Update the properties of a rbacApplication object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update rbacApplication

Namespace: Microsoft.DirectoryServices

Update the properties of a [rbacApplication](../resources/microsoft.directoryservices-rbacapplication.md) object.

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
PATCH /roleManagement/directory
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [rbacApplication](../resources/microsoft.directoryservices-rbacapplication.md) object.

The following table shows the properties that are required when you create the [rbacApplication](../resources/microsoft.directoryservices-rbacapplication.md).

|Property|Type|Description|
|:---|:---|:---|



## Response
If successful, this method returns a `200 OK` response code and an updated [rbacApplication](../resources/microsoft.directoryservices-rbacapplication.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_rbacapplication"
}
-->
``` http
PATCH https://graph.microsoft.com/changelog/roleManagement/directory
Content-Type: application/json
Content-length: 69

{
  "@odata.type": "#Microsoft.DirectoryServices.rbacApplication"
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
  "@odata.type": "#Microsoft.DirectoryServices.rbacApplication"
}
```

