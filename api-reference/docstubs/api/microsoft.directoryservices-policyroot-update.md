---
title: "Update policyRoot"
description: "Update the properties of a policyRoot object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update policyRoot

Namespace: microsoft.DirectoryServices

Update the properties of a [policyRoot](../resources/microsoft.directoryservices-policyroot.md) object.

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
PATCH /policies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [policyRoot](../resources/microsoft.directoryservices-policyroot.md) object.

The following table shows the properties that are required when you create the [policyRoot](../resources/microsoft.directoryservices-policyroot.md).

|Property|Type|Description|
|:---|:---|:---|



## Response
If successful, this method returns a `200 OK` response code and an updated [policyRoot](../resources/microsoft.directoryservices-policyroot.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_policyroot"
}
-->
``` http
PATCH https://graph.microsoft.com/changelog/policies
Content-Type: application/json
Content-length: 64

{
  "@odata.type": "#microsoft.DirectoryServices.policyRoot"
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
  "@odata.type": "#microsoft.DirectoryServices.policyRoot"
}
```

