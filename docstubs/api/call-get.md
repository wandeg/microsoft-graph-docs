---
title: "Get call"
description: "Read properties and relationships of the call object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get call

Namespace: microsoft.graph

Read properties and relationships of the [call](../resources/call.md) object.

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
GET /app/calls/{callId}
GET /communications/calls/{callId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [call](../resources/call.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_call"
}
-->
``` http
GET https://graph.microsoft.com/beta/app/calls/{callId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3417

{
  "value": {
    "@odata.type": "#microsoft.graph.call",
    "id": "2c479e96-9e96-2c47-969e-472c969e472c",
    "state": "String",
    "mediaState": {
      "@odata.type": "microsoft.graph.callMediaState",
      "audio": "String"
    },
    "resultInfo": {
      "@odata.type": "microsoft.graph.ResultInfo",
      "code": 4,
      "subcode": 7,
      "message": "Message value"
    },
    "terminationReason": "Termination Reason value",
    "direction": "String",
    "ringingTimeoutInSeconds": 7,
    "subject": "Subject value",
    "callbackUri": "Callback Uri value",
    "callRoutes": [
      {
        "@odata.type": "microsoft.graph.callRoute",
        "routingType": "String",
        "original": {
          "@odata.type": "microsoft.graph.identitySet",
          "application": {
            "@odata.type": "microsoft.graph.identity",
            "id": "Id value",
            "displayName": "Display Name value"
          },
          "device": {
            "@odata.type": "microsoft.graph.identity"
          },
          "user": {
            "@odata.type": "microsoft.graph.identity"
          }
        },
        "final": {
          "@odata.type": "microsoft.graph.identitySet"
        }
      }
    ],
    "source": {
      "@odata.type": "microsoft.graph.participantInfo",
      "identity": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "endpointType": "String",
      "region": "Region value",
      "languageId": "Language Id value",
      "countryCode": "Country Code value"
    },
    "targets": [
      {
        "@odata.type": "microsoft.graph.invitationParticipantInfo",
        "replacesCallId": "Replaces Call Id value"
      }
    ],
    "answeredBy": {
      "@odata.type": "microsoft.graph.participantInfo"
    },
    "requestedModalities": [
      "String"
    ],
    "activeModalities": [
      "String"
    ],
    "mediaConfig": {
      "@odata.type": "microsoft.graph.mediaConfig",
      "removeFromDefaultAudioGroup": true
    },
    "chatInfo": {
      "@odata.type": "microsoft.graph.chatInfo",
      "threadId": "Thread Id value",
      "messageId": "Message Id value",
      "replyChainMessageId": "Reply Chain Message Id value"
    },
    "callOptions": {
      "@odata.type": "microsoft.graph.callOptions"
    },
    "meetingInfo": {
      "@odata.type": "microsoft.graph.meetingInfo",
      "allowConversationWithoutHost": true
    },
    "meetingCapability": {
      "@odata.type": "microsoft.graph.meetingCapability",
      "allowAnonymousUsersToDialOut": true,
      "autoAdmittedUsers": "String",
      "allowAnonymousUsersToStartMeeting": true
    },
    "routingPolicies": [
      "String"
    ],
    "tenantId": "Tenant Id value",
    "myParticipantId": "My Participant Id value",
    "toneInfo": {
      "@odata.type": "microsoft.graph.toneInfo",
      "sequenceId": 10,
      "tone": "String"
    },
    "callChainId": "Call Chain Id value",
    "incomingContext": {
      "@odata.type": "microsoft.graph.incomingContext",
      "sourceParticipantId": "Source Participant Id value",
      "observedParticipantId": "Observed Participant Id value",
      "onBehalfOf": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "transferor": {
        "@odata.type": "microsoft.graph.identitySet"
      }
    }
  }
}
```

