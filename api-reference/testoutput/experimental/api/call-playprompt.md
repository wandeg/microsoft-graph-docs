---
title: "playPrompt"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# playPrompt



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
POST /app/calls/{callId}/playPrompt
POST /communications/calls/{callId}/playPrompt
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|prompts|[prompt](../resources/prompt.md) collection||
|loop|Boolean||
|clientContext|String||



## Response
If successful, this action returns a `200 OK` response code and a [playPromptOperation](../resources/playPromptOperation.md) in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "call_playprompt"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/app/calls/{callId}/playPrompt

Content-type: application/json
Content-length: 327

{
  "prompts": [
    {
      "@odata.type": "microsoft.graph.mediaPrompt",
      "mediaInfo": {
        "@odata.type": "microsoft.graph.mediaInfo",
        "uri": "Uri value",
        "resourceId": "Resource Id value"
      },
      "loop": 4
    }
  ],
  "loop": true,
  "clientContext": "Client Context value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.playpromptoperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 319

{
  "value": {
    "@odata.type": "#microsoft.graph.playPromptOperation",
    "id": "2cb4b04a-b04a-2cb4-4ab0-b42c4ab0b42c",
    "status": "String",
    "clientContext": "Client Context value",
    "resultInfo": {
      "@odata.type": "microsoft.graph.ResultInfo"
    },
    "completionReason": "String"
  }
}
```

