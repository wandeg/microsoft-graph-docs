---
title: "Update operation"
description: "Update the properties of a operation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update operation

Update the properties of a [operation](../resources/operation.md) object.

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
PATCH ** Entity URI for microsoft.graph.operation not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

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
If successful, this method returns a `200 OK` response code and an updated [operation](../resources/operation.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_operation"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.operation not found
Content-type: application/json
Content-length: 136

{
  "@odata.type": "#microsoft.graph.operation",
  "status": "String",
  "lastActionDateTime": "2017-01-01T00:01:23.8467386+03:00"
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
Content-Length: 244

{
  "@odata.type": "#microsoft.graph.operation",
  "id": "b9c58abd-8abd-b9c5-bd8a-c5b9bd8ac5b9",
  "status": "String",
  "createdDateTime": "2016-12-31T23:57:22.3554145+03:00",
  "lastActionDateTime": "2017-01-01T00:01:23.8467386+03:00"
}
```

