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

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /impossibleTravelRiskEvents
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
If successful, this method returns a `200 OK` response code and a collection of [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_impossibletravelriskevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/impossibleTravelRiskEvents
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
Content-Length: 1407

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.impossibleTravelRiskEvent",
      "id": "cfadd5a8-d5a8-cfad-a8d5-adcfa8d5adcf",
      "userDisplayName": "User Display Name value",
      "userPrincipalName": "User Principal Name value",
      "riskEventDateTime": "2017-01-01T00:01:29.3606209+03:00",
      "riskEventType": "Risk Event Type value",
      "riskLevel": "String",
      "riskEventStatus": "String",
      "closedDateTime": "2017-01-01T00:00:28.7472942+03:00",
      "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
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
      "previousSigninDateTime": "2017-01-01T00:00:31.1907923+03:00",
      "previousLocation": {
        "@odata.type": "microsoft.graph.signInLocation"
      },
      "previousIpAddress": "Previous Ip Address value"
    }
  ]
}
```

