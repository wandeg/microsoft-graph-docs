---
title: "call: record"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# record

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
POST /app/calls/{callId}/record
POST /communications/calls/{callId}/record
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
|bargeInAllowed|Boolean|**TODO: Add Description**|
|initialSilenceTimeoutInSeconds|Int32|**TODO: Add Description**|
|maxSilenceTimeoutInSeconds|Int32|**TODO: Add Description**|
|maxRecordDurationInSeconds|Int32|**TODO: Add Description**|
|playBeep|Boolean|**TODO: Add Description**|
|streamWhileRecording|Boolean|**TODO: Add Description**|
|stopTones|String collection|**TODO: Add Description**|
|clientContext|String|**TODO: Add Description**|



## Response
If successful, this action returns a `200 OK` response code and a [recordOperation](../resources/recordoperation.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "call_record"
}
-->
``` http
POST https://graph.microsoft.com/beta/app/calls/{callId}/record

Content-Type: application/json
Content-length: 379

{
  "prompts": [
    {
      "@odata.type": "microsoft.graph.mediaPrompt"
    }
  ],
  "bargeInAllowed": true,
  "initialSilenceTimeoutInSeconds": 14,
  "maxSilenceTimeoutInSeconds": 10,
  "maxRecordDurationInSeconds": 10,
  "playBeep": true,
  "streamWhileRecording": true,
  "stopTones": [
    "Stop Tones value"
  ],
  "clientContext": "Client Context value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordoperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.recordOperation",
    "id": "5fb89799-9799-5fb8-9997-b85f9997b85f",
    "status": "String",
    "clientContext": "Client Context value",
    "resultInfo": {
      "@odata.type": "microsoft.graph.ResultInfo"
    },
    "recordingLocation": "Recording Location value",
    "recordingAccessToken": "Recording Access Token value",
    "completionReason": "String"
  }
}
```

