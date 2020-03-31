---
title: "Get leakedCredentialsRiskEvent"
description: "Read properties and relationships of the leakedCredentialsRiskEvent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get leakedCredentialsRiskEvent

Namespace: microsoft.graph

Read properties and relationships of the [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object.

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
GET /leakedCredentialsRiskEvents/{leakedCredentialsRiskEventsId}
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
If successful, this method returns a `200 OK` response code and [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/leakedCredentialsRiskEvents/{leakedCredentialsRiskEventsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 570

{
  "value": {
    "@odata.type": "#microsoft.graph.leakedCredentialsRiskEvent",
    "id": "854e687b-687b-854e-7b68-4e857b684e85",
    "userDisplayName": "User Display Name value",
    "userPrincipalName": "User Principal Name value",
    "riskEventDateTime": "2016-12-31T23:59:24.8510287+03:00",
    "riskEventType": "Risk Event Type value",
    "riskLevel": "String",
    "riskEventStatus": "String",
    "closedDateTime": "2016-12-31T23:59:32.6411881+03:00",
    "createdDateTime": "2017-01-01T00:01:55.391884+03:00",
    "userId": "User Id value"
  }
}
```

