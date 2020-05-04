---
title: "Create calls"
description: "Create a new calls object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create calls

Namespace: microsoft.graph

Create a new calls object.

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
POST /communications/calls
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [call](../resources/call.md) object.

The following table shows the properties that are required when you create the [call](../resources/call.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|state|callState|**TODO: Add Description**. Possible values are: `incoming`, `establishing`, `ringing`, `established`, `hold`, `transferring`, `transferAccepted`, `redirecting`, `terminating`, `terminated`, `unknownFutureValue`.|
|mediaState|[callMediaState](../resources/callmediastate.md)|**TODO: Add Description**|
|resultInfo|[ResultInfo](../resources/resultinfo.md)|**TODO: Add Description**|
|terminationReason|String|**TODO: Add Description**|
|direction|callDirection|**TODO: Add Description**. Possible values are: `incoming`, `outgoing`.|
|ringingTimeoutInSeconds|Int32|**TODO: Add Description**|
|subject|String|**TODO: Add Description**|
|callbackUri|String|**TODO: Add Description**|
|callRoutes|[callRoute](../resources/callroute.md) collection|**TODO: Add Description**|
|source|[participantInfo](../resources/participantinfo.md)|**TODO: Add Description**|
|targets|[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection|**TODO: Add Description**|
|answeredBy|[participantInfo](../resources/participantinfo.md)|**TODO: Add Description**|
|requestedModalities|modality collection|**TODO: Add Description**. Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `unknownFutureValue`.|
|activeModalities|modality collection|**TODO: Add Description**. Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `unknownFutureValue`.|
|mediaConfig|[mediaConfig](../resources/mediaconfig.md)|**TODO: Add Description**|
|chatInfo|[chatInfo](../resources/chatinfo.md)|**TODO: Add Description**|
|callOptions|[callOptions](../resources/calloptions.md)|**TODO: Add Description**|
|meetingInfo|[meetingInfo](../resources/meetinginfo.md)|**TODO: Add Description**|
|meetingCapability|[meetingCapability](../resources/meetingcapability.md)|**TODO: Add Description**|
|routingPolicies|routingPolicy collection|**TODO: Add Description**. Possible values are: `none`, `noMissedCall`, `disableForwardingExceptPhone`, `disableForwarding`, `preferSkypeForBusiness`, `unknownFutureValue`.|
|tenantId|String|**TODO: Add Description**|
|myParticipantId|String|**TODO: Add Description**|
|toneInfo|[toneInfo](../resources/toneinfo.md)|**TODO: Add Description**|
|incomingContext|[incomingContext](../resources/incomingcontext.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_call_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json
Content-length: 3086

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
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
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
```

