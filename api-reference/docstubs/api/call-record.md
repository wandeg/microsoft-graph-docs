---
title: "call: record"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
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
POST https://graph.microsoft.com/beta/communications/calls/{callId}/record

Content-Type: application/json
Content-length: 346

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
  "stopTones": [
    "Stop Tones value"
  ],
  "clientContext": "Client Context value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
    "id": "c13ba64d-a64d-c13b-4da6-3bc14da63bc1",
    "status": "String",
    "clientContext": "Client Context value",
    "resultInfo": {
      "@odata.type": "microsoft.graph.resultInfo"
    },
    "recordingLocation": "Recording Location value",
    "recordingAccessToken": "Recording Access Token value"
  }
}
```

