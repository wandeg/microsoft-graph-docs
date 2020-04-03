---
title: "Get anonymousIpRiskEvent"
description: "Read properties and relationships of the anonymousIpRiskEvent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get anonymousIpRiskEvent

Namespace: microsoft.graph

Read properties and relationships of the [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object.

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
GET /anonymousIpRiskEvents/{anonymousIpRiskEventsId}
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
If successful, this method returns a `200 OK` response code and [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_anonymousipriskevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/anonymousIpRiskEvents/{anonymousIpRiskEventsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 986

{
  "value": {
    "@odata.type": "#microsoft.graph.anonymousIpRiskEvent",
    "id": "b39053b5-53b5-b390-b553-90b3b55390b3",
    "userDisplayName": "User Display Name value",
    "userPrincipalName": "User Principal Name value",
    "riskEventDateTime": "2016-12-31T23:59:10.9176809+00:00",
    "riskEventType": "Risk Event Type value",
    "riskLevel": "String",
    "riskEventStatus": "String",
    "closedDateTime": "2016-12-31T23:59:20.3348093+00:00",
    "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
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

