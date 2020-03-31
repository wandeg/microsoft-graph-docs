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
POST /connections/{connectionsId}/operations/$ref
POST /external/connections/{externalConnectionId}/operations/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [connectionOperation](../resources/connectionoperation.md) object.

The following table shows the properties that are required when you create the [connectionOperation](../resources/connectionoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|status|Enumeration| Possible values are: `unspecified`, `inprogress`, `completed`, `failed`.|
|error|[errorDetail](../resources/errordetail.md)||



## Response
If successful, this method returns a `201 Created` response code and a [connectionOperation](../resources/connectionoperation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_connectionoperation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/connections/{connectionsId}/operations
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
  "truncated": true,
  "@odata.type": "microsoft.graph.connectionoperation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 412

{
  "@odata.type": "#microsoft.graph.connectionOperation",
  "id": "f11e4f67-4f67-f11e-674f-1ef1674f1ef1",
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

