---
title: "Update muteParticipantsOperation"
description: "Update the properties of a muteParticipantsOperation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update muteParticipantsOperation

Update the properties of a [muteParticipantsOperation](../resources/muteparticipantsoperation.md) object.

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
PATCH ** Entity URI for microsoft.graph.muteParticipantsOperation not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [muteParticipantsOperation](../resources/muteParticipantsOperation.md) object.

The following table shows the properties that are required when you create the [muteParticipantsOperation](../resources/muteparticipantsoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|status|Enumeration| Inherited from [commsOperation](../resources/commsOperation.md). Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|
|clientContext|String| Inherited from [commsOperation](../resources/commsOperation.md)|
|resultInfo|[ResultInfo](../resources/ResultInfo.md)| Inherited from [commsOperation](../resources/commsOperation.md)|
|participants|String collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [muteParticipantsOperation](../resources/muteparticipantsoperation.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_muteparticipantsoperation"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.muteParticipantsOperation not found
Content-type: application/json
Content-length: 329

{
  "@odata.type": "#microsoft.graph.muteParticipantsOperation",
  "status": "String",
  "clientContext": "Client Context value",
  "resultInfo": {
    "@odata.type": "microsoft.graph.ResultInfo",
    "code": 4,
    "subcode": 7,
    "message": "Message value"
  },
  "participants": [
    "Participants value"
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 378

{
  "@odata.type": "#microsoft.graph.muteParticipantsOperation",
  "id": "d4ae93cf-93cf-d4ae-cf93-aed4cf93aed4",
  "status": "String",
  "clientContext": "Client Context value",
  "resultInfo": {
    "@odata.type": "microsoft.graph.ResultInfo",
    "code": 4,
    "subcode": 7,
    "message": "Message value"
  },
  "participants": [
    "Participants value"
  ]
}
```

