---
title: "Get riskDetection"
description: "Read the properties and relationships of a riskDetection object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get riskDetection

Namespace: microsoft.graph

Read the properties and relationships of a [riskDetection](../resources/riskdetection.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

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
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [riskDetection](../resources/riskdetection.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_riskdetection"
}
-->
``` http
GET https://graph.microsoft.com/beta/riskDetections/{riskDetectionsId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskDetection"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.riskDetection",
    "id": "b5a8acc2-acc2-b5a8-c2ac-a8b5c2aca8b5",
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
    "activityDateTime": "2017-01-01T00:03:07.3452024+03:00",
    "detectedDateTime": "2016-12-31T23:59:49.2842106+03:00",
    "lastUpdatedDateTime": "2016-12-31T23:58:57.2159356+03:00",
    "userId": "User Id value",
    "userDisplayName": "User Display Name value",
    "userPrincipalName": "User Principal Name value",
    "additionalInfo": "Additional Info value"
  }
}
```

