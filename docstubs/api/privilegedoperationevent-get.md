---
title: "Get privilegedOperationEvent"
description: "Read properties and relationships of the privilegedOperationEvent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get privilegedOperationEvent

Namespace: microsoft.graph

Read properties and relationships of the [privilegedOperationEvent](../resources/privilegedoperationevent.md) object.

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
GET /privilegedOperationEvents/{privilegedOperationEventsId}
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
If successful, this method returns a `200 OK` response code and [privilegedOperationEvent](../resources/privilegedoperationevent.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_privilegedoperationevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/privilegedOperationEvents/{privilegedOperationEventsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedOperationEvent"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 757

{
  "value": {
    "@odata.type": "#microsoft.graph.privilegedOperationEvent",
    "id": "4ac0af35-af35-4ac0-35af-c04a35afc04a",
    "userId": "User Id value",
    "userName": "User Name value",
    "userMail": "User Mail value",
    "roleId": "Role Id value",
    "roleName": "Role Name value",
    "expirationDateTime": "2016-12-31T23:57:47.0232285+00:00",
    "creationDateTime": "2017-01-01T00:02:18.736171+00:00",
    "requestorId": "Requestor Id value",
    "requestorName": "Requestor Name value",
    "tenantId": "Tenant Id value",
    "requestType": "Request Type value",
    "additionalInformation": "Additional Information value",
    "referenceKey": "Reference Key value",
    "referenceSystem": "Reference System value"
  }
}
```

