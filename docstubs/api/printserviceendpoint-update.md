---
title: "Update printServiceEndpoint"
description: "Update the properties of a printServiceEndpoint object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update printServiceEndpoint

Namespace: microsoft.graph

Update the properties of a [printServiceEndpoint](../resources/printserviceendpoint.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/services/{printServiceId}/endpoints/{printServiceEndpointId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [printServiceEndpoint](../resources/printserviceendpoint.md) object.

The following table shows the properties that are required when you create the [printServiceEndpoint](../resources/printserviceendpoint.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|uri|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [printServiceEndpoint](../resources/printserviceendpoint.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_printserviceendpoint"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/print/services/{printServiceId}/endpoints/{printServiceEndpointId}
Content-type: application/json
Content-length: 125

{
  "@odata.type": "#microsoft.graph.printServiceEndpoint",
  "displayName": "Display Name value",
  "uri": "Uri value"
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
Content-Length: 174

{
  "@odata.type": "#microsoft.graph.printServiceEndpoint",
  "id": "db37e856-e856-db37-56e8-37db56e837db",
  "displayName": "Display Name value",
  "uri": "Uri value"
}
```

