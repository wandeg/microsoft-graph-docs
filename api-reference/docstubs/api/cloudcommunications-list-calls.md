---
title: "List calls"
description: "Get the calls from the calls navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List calls

Namespace: microsoft.graph

Get the calls from the calls navigation property.

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
GET /communications/calls
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [call](../resources/call.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_call"
}
-->
``` http
GET https://graph.microsoft.com/beta/communications/calls
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.call)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.call",
      "id": "93f47936-7936-93f4-3679-f4933679f493",
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
  ]
}
```

