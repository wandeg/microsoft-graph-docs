---
title: "invite"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# invite

Namespace: microsoft.graph



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
POST /app/calls/{callId}/participants/invite
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|participants|[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection||
|clientContext|String||



## Response
If successful, this action returns a `200 OK` response code and a [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "participant_invite"
}
-->
``` http
POST https://graph.microsoft.com/beta/app/calls/{callId}/participants/invite

Content-type: application/json
Content-length: 154

{
  "participants": [
    {
      "@odata.type": "microsoft.graph.invitationParticipantInfo"
    }
  ],
  "clientContext": "Client Context value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inviteparticipantsoperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "value": {
    "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
    "id": "57bf2dc0-2dc0-57bf-c02d-bf57c02dbf57",
    "status": "String",
    "clientContext": "Client Context value",
    "resultInfo": {
      "@odata.type": "microsoft.graph.ResultInfo"
    },
    "participants": [
      {
        "@odata.type": "microsoft.graph.invitationParticipantInfo"
      }
    ]
  }
}
```

