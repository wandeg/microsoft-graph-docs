---
title: "List calls"
description: "Get the calls from the calls navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List calls

Namespace: microsoft.graph

Get the calls from the calls navigation property.

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
GET /communications/calls
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [call](../resources/call.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_call"
}
-->
``` http
GET https://graph.microsoft.com/localtest/communications/calls
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.call)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1975

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.call",
      "id": "5b064ea4-4ea4-5b06-a44e-065ba44e065b",
      "state": "String",
      "mediaState": {
        "@odata.type": "microsoft.graph.callMediaState",
        "audio": "String"
      },
      "resultInfo": {
        "@odata.type": "microsoft.graph.resultInfo",
        "code": 4,
        "subcode": 7,
        "message": "Message value"
      },
      "direction": "String",
      "subject": "Subject value",
      "callbackUri": "Callback Uri value",
      "source": {
        "@odata.type": "microsoft.graph.participantInfo",
        "identity": {
          "@odata.type": "microsoft.graph.identitySet",
          "application": {
            "@odata.type": "microsoft.graph.identity",
            "displayName": "Display Name value",
            "id": "Id value"
          },
          "device": {
            "@odata.type": "microsoft.graph.identity"
          },
          "user": {
            "@odata.type": "microsoft.graph.identity"
          }
        },
        "region": "Region value",
        "languageId": "Language Id value"
      },
      "targets": [
        {
          "@odata.type": "microsoft.graph.participantInfo"
        }
      ],
      "requestedModalities": [
        "String"
      ],
      "mediaConfig": {
        "@odata.type": "microsoft.graph.mediaConfig"
      },
      "chatInfo": {
        "@odata.type": "microsoft.graph.chatInfo",
        "threadId": "Thread Id value",
        "messageId": "Message Id value",
        "replyChainMessageId": "Reply Chain Message Id value"
      },
      "meetingInfo": {
        "@odata.type": "microsoft.graph.meetingInfo"
      },
      "tenantId": "Tenant Id value",
      "myParticipantId": "My Participant Id value",
      "toneInfo": {
        "@odata.type": "microsoft.graph.toneInfo",
        "sequenceId": 10,
        "tone": "String"
      }
    }
  ]
}
```

