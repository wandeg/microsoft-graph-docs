---
title: "Update connectionOperation"
description: "Update the properties of a connectionOperation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update connectionOperation

Namespace: microsoft.graph

Update the properties of a [connectionOperation](../resources/connectionoperation.md) object.

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
PATCH /connections/{connectionsId}/operations/{connectionOperationId}
PATCH /external/connections/{externalConnectionId}/operations/{connectionOperationId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [connectionOperation](../resources/connectionoperation.md) object.

The following table shows the properties that are required when you create the [connectionOperation](../resources/connectionoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|status|Enumeration|. Possible values are: `unspecified`, `inprogress`, `completed`, `failed`.|
|error|[errorDetail](../resources/errordetail.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [connectionOperation](../resources/connectionoperation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_connectionoperation"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/connections/{connectionsId}/operations/{connectionOperationId}
Content-type: application/json
Content-length: 363

{
  "@odata.type": "#microsoft.graph.connectionOperation",
  "status": "String",
  "error": {
    "@odata.type": "microsoft.graph.errorDetail",
    "errorCode": "Error Code value",
    "message": "Message value",
    "details": [
      {
        "@odata.type": "microsoft.graph.innerErrorDetail",
        "source": "Source value"
      }
    ]
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
Content-Length: 412

{
  "@odata.type": "#microsoft.graph.connectionOperation",
  "id": "c2915c4b-5c4b-c291-4b5c-91c24b5c91c2",
  "status": "String",
  "error": {
    "@odata.type": "microsoft.graph.errorDetail",
    "errorCode": "Error Code value",
    "message": "Message value",
    "details": [
      {
        "@odata.type": "microsoft.graph.innerErrorDetail",
        "source": "Source value"
      }
    ]
  }
}
```

