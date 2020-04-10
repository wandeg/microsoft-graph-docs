---
title: "Add endpoints"
description: "Add endpoints by posting to the endpoints collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add endpoints

Namespace: microsoft.graph

Add endpoints by posting to the endpoints collection.

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
POST /print/services/{printServiceId}/endpoints/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [printServiceEndpoint](../resources/printserviceendpoint.md) object.

The following table shows the properties that are required when you create the [printServiceEndpoint](../resources/printserviceendpoint.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|uri|String||



## Response
If successful, this method returns a `201 Created` response code and a [printServiceEndpoint](../resources/printserviceendpoint.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_printserviceendpoint_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/print/services/{printServiceId}/endpoints
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
  "truncated": true,
  "@odata.type": "microsoft.graph.printserviceendpoint"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 174

{
  "@odata.type": "#microsoft.graph.printServiceEndpoint",
  "id": "db37e856-e856-db37-56e8-37db56e837db",
  "displayName": "Display Name value",
  "uri": "Uri value"
}
```

