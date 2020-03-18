---
title: "Add operations"
description: "Add operations by posting to the operations collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add operations

Namespace: microsoft.graph

Add operations by posting to the operations collection.

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
POST /me/onenote/operations/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [onenoteOperation](../resources/onenoteoperation.md) object.

The following table shows the properties that are required when you create the [onenoteOperation](../resources/onenoteoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|status|Enumeration| Inherited from [operation](../resources/operation.md). Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|
|createdDateTime|DateTimeOffset| Inherited from [operation](../resources/operation.md)|
|lastActionDateTime|DateTimeOffset| Inherited from [operation](../resources/operation.md)|
|resourceLocation|String||
|resourceId|String||
|error|[onenoteOperationError](../resources/onenoteoperationerror.md)||
|percentComplete|String||



## Response
If successful, this method returns a `201 Created` response code and a [onenoteOperation](../resources/onenoteoperation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_onenoteoperation_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/onenote/operations
Content-type: application/json
Content-length: 419

{
  "@odata.type": "#microsoft.graph.onenoteOperation",
  "status": "String",
  "lastActionDateTime": "2017-01-01T00:00:06.3761313+03:00",
  "resourceLocation": "Resource Location value",
  "resourceId": "Resource Id value",
  "error": {
    "@odata.type": "microsoft.graph.onenoteOperationError",
    "code": "Code value",
    "message": "Message value"
  },
  "percentComplete": "Percent Complete value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteoperation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 527

{
  "@odata.type": "#microsoft.graph.onenoteOperation",
  "id": "08fa4fcd-4fcd-08fa-cd4f-fa08cd4ffa08",
  "status": "String",
  "createdDateTime": "2017-01-01T00:00:51.2796212+03:00",
  "lastActionDateTime": "2017-01-01T00:00:06.3761313+03:00",
  "resourceLocation": "Resource Location value",
  "resourceId": "Resource Id value",
  "error": {
    "@odata.type": "microsoft.graph.onenoteOperationError",
    "code": "Code value",
    "message": "Message value"
  },
  "percentComplete": "Percent Complete value"
}
```

