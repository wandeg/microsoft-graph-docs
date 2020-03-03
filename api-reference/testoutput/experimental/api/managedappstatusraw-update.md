---
title: "Update managedAppStatusRaw"
description: "Update the properties of a managedAppStatusRaw object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update managedAppStatusRaw

Update the properties of a [managedAppStatusRaw](../resources/managedappstatusraw.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH ** Entity URI for microsoft.graph.managedAppStatusRaw not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [managedAppStatusRaw](../resources/managedAppStatusRaw.md) object.

The following table shows the properties that are required when you create the [managedAppStatusRaw](../resources/managedappstatusraw.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|Friendly name of the status report. Inherited from [managedAppStatus](../resources/managedAppStatus.md)|
|version|String|Version of the entity. Inherited from [managedAppStatus](../resources/managedAppStatus.md)|
|content|[Json](../resources/Json.md)|Status report content.|



## Response
If successful, this method returns a `200 OK` response code and an updated [managedAppStatusRaw](../resources/managedappstatusraw.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_managedappstatusraw"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.managedAppStatusRaw not found
Content-type: application/json
Content-length: 197

{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "Display Name value",
  "version": "Version value",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 246

{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "id": "16795e66-5e66-1679-665e-7916665e7916",
  "displayName": "Display Name value",
  "version": "Version value",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

