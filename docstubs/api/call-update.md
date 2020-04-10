---
title: "Update call"
description: "Update the properties of a call object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update call

Namespace: microsoft.graph

Update the properties of a [call](../resources/call.md) object.

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
PATCH /app/calls/{callId}
PATCH /communications/calls/{callId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [call](../resources/call.md) object.

The following table shows the properties that are required when you create the [call](../resources/call.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|state|Enumeration| Possible values are: `incoming`, `establishing`, `ringing`, `established`, `hold`, `transferring`, `transferAccepted`, `redirecting`, `terminating`, `terminated`, `unknownFutureValue`.|
|mediaState|[callMediaState](../resources/callmediastate.md)||
|resultInfo|[ResultInfo](../resources/resultinfo.md)||
|terminationReason|String||
|direction|Enumeration| Possible values are: `incoming`, `outgoing`.|
|ringingTimeoutInSeconds|Int32||
|subject|String||
|callbackUri|String||
|callRoutes|[callRoute](../resources/callroute.md) collection||
|source|[participantInfo](../resources/participantinfo.md)||
|targets|[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection||
|answeredBy|[participantInfo](../resources/participantinfo.md)||
|requestedModalities|Enumeration collection| Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `unknownFutureValue`.|
|activeModalities|Enumeration collection| Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `unknownFutureValue`.|
|mediaConfig|[mediaConfig](../resources/mediaconfig.md)||
|chatInfo|[chatInfo](../resources/chatinfo.md)||
|callOptions|[callOptions](../resources/calloptions.md)||
|meetingInfo|[meetingInfo](../resources/meetinginfo.md)||
|meetingCapability|[meetingCapability](../resources/meetingcapability.md)||
|routingPolicies|Enumeration collection| Possible values are: `none`, `noMissedCall`, `disableForwardingExceptPhone`, `disableForwarding`, `preferSkypeForBusiness`, `unknownFutureValue`.|
|tenantId|String||
|myParticipantId|String||
|toneInfo|[toneInfo](../resources/toneinfo.md)||
|callChainId|String||
|incomingContext|[incomingContext](../resources/incomingcontext.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [call](../resources/call.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_call"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/app/calls/{callId}
Content-type: application/json
Content-length: 3127

{
  "@odata.type": "#microsoft.graph.call",
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
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3176

{
  "@odata.type": "#microsoft.graph.call",
  "id": "ae373e90-3e90-ae37-903e-37ae903e37ae",
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
```

