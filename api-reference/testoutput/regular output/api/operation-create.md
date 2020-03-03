---
title: "Create operation"
description: "Create a new operation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create operation

Namespace: microsoft.graph

Create a new [operation](../resources/operation.md) object.

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
POST ** Collection URI for microsoft.graph.operation not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [operation](../resources/operation.md) object.

The following table shows the properties that are required when you create the [operation](../resources/operation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|status|Enumeration|. Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|
|createdDateTime|DateTimeOffset||
|lastActionDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [operation](../resources/operation.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_operation_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.operation not found
Content-type: application/json
Content-length: 136

{
  "@odata.type": "#microsoft.graph.operation",
  "status": "String",
  "lastActionDateTime": "2017-01-01T00:02:27.6832592+03:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.operation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 243

{
  "@odata.type": "#microsoft.graph.operation",
  "id": "7986a22f-a22f-7986-2fa2-86792fa28679",
  "status": "String",
  "createdDateTime": "2017-01-01T00:02:24.618735+03:00",
  "lastActionDateTime": "2017-01-01T00:02:27.6832592+03:00"
}
```

