---
title: "cancelMediaProcessing"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# cancelMediaProcessing

Namespace: microsoft.graph



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
POST /app/calls/{callId}/cancelMediaProcessing
POST /communications/calls/{callId}/cancelMediaProcessing
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|clientContext|String||



## Response
If successful, this action returns a `200 OK` response code and a [cancelMediaProcessingOperation](../resources/cancelmediaprocessingoperation.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "call_cancelmediaprocessing"
}
-->
``` http
POST https://graph.microsoft.com/beta/app/calls/{callId}/cancelMediaProcessing

Content-type: application/json
Content-length: 47

{
  "clientContext": "Client Context value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cancelmediaprocessingoperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "value": {
    "@odata.type": "#microsoft.graph.cancelMediaProcessingOperation",
    "id": "5225eaa6-eaa6-5225-a6ea-2552a6ea2552",
    "status": "String",
    "clientContext": "Client Context value",
    "resultInfo": {
      "@odata.type": "microsoft.graph.ResultInfo"
    }
  }
}
```

