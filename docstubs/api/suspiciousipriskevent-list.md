---
title: "List suspiciousIpRiskEvents"
description: "List properties and relationships of the suspiciousIpRiskEvent objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List suspiciousIpRiskEvents

Namespace: microsoft.graph

List properties and relationships of the [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) objects.

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
GET /suspiciousIpRiskEvents
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
If successful, this method returns a `200 OK` response code and a collection of [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_suspiciousipriskevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/suspiciousIpRiskEvents
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.suspiciousipriskevent)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1049

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.suspiciousIpRiskEvent",
      "id": "298a67f9-67f9-298a-f967-8a29f9678a29",
      "userDisplayName": "User Display Name value",
      "userPrincipalName": "User Principal Name value",
      "riskEventDateTime": "2017-01-01T00:03:28.9237667+00:00",
      "riskEventType": "Risk Event Type value",
      "riskLevel": "String",
      "riskEventStatus": "String",
      "closedDateTime": "2017-01-01T00:02:12.8597976+00:00",
      "createdDateTime": "2016-12-31T23:59:31.6288943+00:00",
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
  ]
}
```

