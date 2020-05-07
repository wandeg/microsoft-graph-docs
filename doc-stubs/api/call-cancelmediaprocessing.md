---
title: "call: cancelMediaProcessing"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# cancelMediaProcessing

Namespace: microsoft.graph

**TODO: Add Description**

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

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
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|clientContext|String|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [cancelMediaProcessingOperation](../resources/cancelmediaprocessingoperation.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "call_cancelmediaprocessing"
}
-->
``` http
POST https://graph.microsoft.com/beta/app/calls/{callId}/cancelMediaProcessing

Content-Type: application/json
Content-length: 33

{
  "clientContext": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cancelmediaprocessingoperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.cancelMediaProcessingOperation",
    "id": "String (identifier)",
    "status": "String",
    "clientContext": "String",
    "resultInfo": {
      "@odata.type": "microsoft.graph.ResultInfo"
    }
  }
}
```

