---
title: "user: exportDeviceAndAppManagementData"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# exportDeviceAndAppManagementData

Namespace: microsoft.graph

**TODO: Add Description**

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
GET /me/exportDeviceAndAppManagementData
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Function parameters
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Parameter|Type|Description|
|:---|:---|:---|
|skip|Int32|**TODO: Add Description**|
|top|Int32|**TODO: Add Description**|



## Response
If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/deviceandappmanagementdata.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "user_exportdeviceandappmanagementdata"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/exportDeviceAndAppManagementData(skip=Integer,top=Integer)
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceandappmanagementdata"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementData"
  }
}
```

