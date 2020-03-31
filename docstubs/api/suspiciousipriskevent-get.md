---
title: "Get suspiciousIpRiskEvent"
description: "Read properties and relationships of the suspiciousIpRiskEvent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get suspiciousIpRiskEvent

Namespace: microsoft.graph

Read properties and relationships of the [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) object.

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
GET /suspiciousIpRiskEvents/{suspiciousIpRiskEventsId}
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
If successful, this method returns a `200 OK` response code and [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_suspiciousipriskevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/suspiciousIpRiskEvents/{suspiciousIpRiskEventsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.suspiciousIpRiskEvent"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 986

{
  "value": {
    "@odata.type": "#microsoft.graph.suspiciousIpRiskEvent",
    "id": "116f01af-01af-116f-af01-6f11af016f11",
    "userDisplayName": "User Display Name value",
    "userPrincipalName": "User Principal Name value",
    "riskEventDateTime": "2016-12-31T23:59:24.8510287+03:00",
    "riskEventType": "Risk Event Type value",
    "riskLevel": "String",
    "riskEventStatus": "String",
    "closedDateTime": "2016-12-31T23:59:32.6411881+03:00",
    "createdDateTime": "2017-01-01T00:01:55.391884+03:00",
    "userId": "User Id value",
    "location": {
      "@odata.type": "microsoft.graph.signInLocation",
      "city": "City value",
      "state": "State value",
      "countryOrRegion": "Country Or Region value",
      "geoCoordinates": {
        "@odata.type": "microsoft.graph.geoCoordinates",
        "altitude": "Double",
        "latitude": "Double",
        "longitude": "Double"
      }
    },
    "ipAddress": "Ip Address value"
  }
}
```

