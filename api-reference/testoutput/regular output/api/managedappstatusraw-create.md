---
title: "Create managedAppStatusRaw"
description: "Create a new managedAppStatusRaw object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create managedAppStatusRaw

Namespace: microsoft.graph

Create a new [managedAppStatusRaw](../resources/managedappstatusraw.md) object.

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
POST ** Collection URI for microsoft.graph.managedAppStatusRaw not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [managedAppStatusRaw](../resources/managedappstatusraw.md) object.

The following table shows the properties that are required when you create the [managedAppStatusRaw](../resources/managedappstatusraw.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|Friendly name of the status report. Inherited from [managedAppStatus](../resources/managedappstatus.md)|
|version|String|Version of the entity. Inherited from [managedAppStatus](../resources/managedappstatus.md)|
|content|[Json](../resources/json.md)|Status report content.|



## Response
If successful, this method returns a `201 Created` response code and a [managedAppStatusRaw](../resources/managedappstatusraw.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_managedappstatusraw_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.managedAppStatusRaw not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.managedappstatusraw"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 246

{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "id": "50cf2147-2147-50cf-4721-cf504721cf50",
  "displayName": "Display Name value",
  "version": "Version value",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

