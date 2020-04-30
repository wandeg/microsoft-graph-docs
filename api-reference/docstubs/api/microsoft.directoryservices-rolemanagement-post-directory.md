---
title: "Create directory"
description: "Create a new directory object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create directory

Namespace: Microsoft.DirectoryServices

Create a new directory object.

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
POST /roleManagement/directory
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [rbacApplication](../resources/microsoft.directoryservices-rbacapplication.md) object.

The following table shows the properties that are required when you create the [rbacApplication](../resources/microsoft.directoryservices-rbacapplication.md).

|Property|Type|Description|
|:---|:---|:---|



## Response
If successful, this method returns a `201 Created` response code and a [rbacApplication](../resources/microsoft.directoryservices-rbacapplication.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_rbacapplication_from_"
}
-->
``` http
POST https://graph.microsoft.com/changelog/roleManagement/directory
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
  "truncated": true,
  "@odata.type": "microsoft.directoryservices.rbacapplication"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.rbacApplication"
}
```

