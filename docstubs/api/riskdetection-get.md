---
title: "Get riskDetection"
description: "Read properties and relationships of the riskDetection object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get riskDetection

Namespace: microsoft.graph

Read properties and relationships of the [riskDetection](../resources/riskdetection.md) object.

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
GET /riskDetections/{riskDetectionsId}
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
If successful, this method returns a `200 OK` response code and [riskDetection](../resources/riskdetection.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_riskdetection"
}
-->
``` http
GET https://graph.microsoft.com/beta/riskDetections/{riskDetectionsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskDetection"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1249

{
  "value": {
    "@odata.type": "#microsoft.graph.riskDetection",
    "id": "65fe6a54-6a54-65fe-546a-fe65546afe65",
    "requestId": "Request Id value",
    "correlationId": "Correlation Id value",
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
    "activityDateTime": "2016-12-31T23:57:31.4887699+00:00",
    "detectedDateTime": "2017-01-01T00:00:36.1709208+00:00",
    "lastUpdatedDateTime": "2016-12-31T23:59:36.3019675+00:00",
    "userId": "User Id value",
    "userDisplayName": "User Display Name value",
    "userPrincipalName": "User Principal Name value",
    "additionalInfo": "Additional Info value"
  }
}
```

