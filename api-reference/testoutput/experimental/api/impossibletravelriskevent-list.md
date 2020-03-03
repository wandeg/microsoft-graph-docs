---
title: "List impossibleTravelRiskEvents"
description: "List properties and relationships of the impossibleTravelRiskEvent objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List impossibleTravelRiskEvents

Namespace: microsoft.graph

List properties and relationships of the [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) objects.

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
GET /impossibleTravelRiskEvents
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_impossibletravelriskevent"
}
-->
``` http
GET https://graph.microsoft.com/localtest/impossibleTravelRiskEvents
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.impossibletravelriskevent)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1406

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.impossibleTravelRiskEvent",
      "id": "ff37d336-d336-ff37-36d3-37ff36d337ff",
      "userDisplayName": "User Display Name value",
      "userPrincipalName": "User Principal Name value",
      "riskEventDateTime": "2017-01-01T00:03:07.0502541+03:00",
      "riskEventType": "Risk Event Type value",
      "riskLevel": "String",
      "riskEventStatus": "String",
      "closedDateTime": "2016-12-31T23:59:27.3956276+03:00",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
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
      "ipAddress": "Ip Address value",
      "userAgent": "User Agent value",
      "deviceInformation": "Device Information value",
      "isAtypicalLocation": true,
      "previousSigninDateTime": "2016-12-31T23:59:31.8597589+03:00",
      "previousLocation": {
        "@odata.type": "microsoft.graph.signInLocation"
      },
      "previousIpAddress": "Previous Ip Address value"
    }
  ]
}
```

