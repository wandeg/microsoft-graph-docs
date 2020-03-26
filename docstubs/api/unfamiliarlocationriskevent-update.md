---
title: "Update unfamiliarLocationRiskEvent"
description: "Update the properties of a unfamiliarLocationRiskEvent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update unfamiliarLocationRiskEvent

Namespace: microsoft.graph

Update the properties of a [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) object.

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
PATCH /unfamiliarLocationRiskEvents/{unfamiliarLocationRiskEventsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) object.

The following table shows the properties that are required when you create the [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userDisplayName|String| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|userPrincipalName|String| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|riskEventDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|riskEventType|String| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|riskLevel|Enumeration| Inherited from [identityRiskEvent](../resources/identityriskevent.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskEventStatus|Enumeration| Inherited from [identityRiskEvent](../resources/identityriskevent.md). Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|closedDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|createdDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|userId|String| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|location|[signInLocation](../resources/signinlocation.md)| Inherited from [locatedRiskEvent](../resources/locatedriskevent.md)|
|ipAddress|String| Inherited from [locatedRiskEvent](../resources/locatedriskevent.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_unfamiliarlocationriskevent"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/unfamiliarLocationRiskEvents/{unfamiliarLocationRiskEventsId}
Content-type: application/json
Content-length: 818

{
  "@odata.type": "#microsoft.graph.unfamiliarLocationRiskEvent",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "riskEventDateTime": "2017-01-01T00:03:28.9237667+00:00",
  "riskEventType": "Risk Event Type value",
  "riskLevel": "String",
  "riskEventStatus": "String",
  "closedDateTime": "2017-01-01T00:02:12.8597976+00:00",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 926

{
  "@odata.type": "#microsoft.graph.unfamiliarLocationRiskEvent",
  "id": "837dff76-ff76-837d-76ff-7d8376ff7d83",
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
```

