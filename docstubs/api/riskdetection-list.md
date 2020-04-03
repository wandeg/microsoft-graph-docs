---
title: "List riskDetections"
description: "List properties and relationships of the riskDetection objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List riskDetections

Namespace: microsoft.graph

List properties and relationships of the [riskDetection](../resources/riskdetection.md) objects.

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
GET /riskDetections
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
If successful, this method returns a `200 OK` response code and a collection of [riskDetection](../resources/riskdetection.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_riskdetection"
}
-->
``` http
GET https://graph.microsoft.com/beta/riskDetections
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.riskdetection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1376

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.riskDetection",
      "id": "64880182-0182-6488-8201-886482018864",
      "requestId": "Request Id value",
      "correlationId": "Correlation Id value",
      "riskEventType": "Risk Event Type value",
      "riskType": "String",
      "riskState": "String",
      "riskLevel": "String",
      "riskDetail": "String",
      "source": "Source value",
      "detectionTimingType": "String",
      "activity": "String",
      "tokenIssuerType": "String",
      "ipAddress": "Ip Address value",
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
      "activityDateTime": "2016-12-31T23:58:36.9952608+00:00",
      "detectedDateTime": "2017-01-01T00:00:16.8903983+00:00",
      "lastUpdatedDateTime": "2016-12-31T23:57:53.6587582+00:00",
      "userId": "User Id value",
      "userDisplayName": "User Display Name value",
      "userPrincipalName": "User Principal Name value",
      "additionalInfo": "Additional Info value"
    }
  ]
}
```

