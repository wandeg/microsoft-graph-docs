---
title: "Get unfamiliarLocationRiskEvent"
description: "Read properties and relationships of the unfamiliarLocationRiskEvent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get unfamiliarLocationRiskEvent

Namespace: microsoft.graph

Read properties and relationships of the [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) object.

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
GET /unfamiliarLocationRiskEvents/{unfamiliarLocationRiskEventsId}
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
If successful, this method returns a `200 OK` response code and [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_unfamiliarlocationriskevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/unfamiliarLocationRiskEvents/{unfamiliarLocationRiskEventsId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unfamiliarLocationRiskEvent"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 992

{
  "value": {
    "@odata.type": "#microsoft.graph.unfamiliarLocationRiskEvent",
    "id": "f3c514b6-14b6-f3c5-b614-c5f3b614c5f3",
    "userDisplayName": "User Display Name value",
    "userPrincipalName": "User Principal Name value",
    "riskEventDateTime": "2017-01-01T00:02:40.748803+00:00",
    "riskEventType": "Risk Event Type value",
    "riskLevel": "String",
    "riskEventStatus": "String",
    "closedDateTime": "2017-01-01T00:01:42.8390447+00:00",
    "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
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

