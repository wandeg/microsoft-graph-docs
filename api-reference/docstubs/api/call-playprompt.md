---
title: "call: playPrompt"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# playPrompt

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
POST /communications/calls/{callId}/playPrompt
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|prompts|[prompt](../resources/prompt.md) collection|**TODO: Add Description**|
|clientContext|String|**TODO: Add Description**|



## Response
If successful, this action returns a `200 OK` response code and a [playPromptOperation](../resources/playpromptoperation.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "call_playprompt"
}
-->
``` http
POST https://graph.microsoft.com/beta/communications/calls/{callId}/playPrompt

Content-Type: application/json
Content-length: 292

{
  "prompts": [
    {
      "@odata.type": "microsoft.graph.mediaPrompt",
      "mediaInfo": {
        "@odata.type": "microsoft.graph.mediaInfo",
        "uri": "Uri value",
        "resourceId": "Resource Id value"
      }
    }
  ],
  "clientContext": "Client Context value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.playpromptoperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.playPromptOperation",
    "id": "1968cc23-cc23-1968-23cc-681923cc6819",
    "status": "String",
    "clientContext": "Client Context value",
    "resultInfo": {
      "@odata.type": "microsoft.graph.resultInfo"
    }
  }
}
```

