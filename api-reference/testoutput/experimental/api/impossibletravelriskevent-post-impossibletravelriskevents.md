---
title: "Create impossibleTravelRiskEvent"
description: "Create a new impossibleTravelRiskEvent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create impossibleTravelRiskEvent

Namespace: microsoft.graph

Create a new [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) object.

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
POST /impossibleTravelRiskEvents
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) object.

The following table shows the properties that are required when you create the [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md).

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
|userAgent|String||
|deviceInformation|String||
|isAtypicalLocation|Boolean||
|previousSigninDateTime|DateTimeOffset||
|previousLocation|[signInLocation](../resources/signinlocation.md)||
|previousIpAddress|String||



## Response
If successful, this method returns a `201 Created` response code and a [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_impossibletravelriskevent_from_impossibletravelriskevents"
}
-->
``` http
POST https://graph.microsoft.com/localtest/impossibleTravelRiskEvents
Content-type: application/json
Content-length: 1138

{
  "@odata.type": "#microsoft.graph.impossibleTravelRiskEvent",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "riskEventDateTime": "2017-01-01T00:03:07.0502541+03:00",
  "riskEventType": "Risk Event Type value",
  "riskLevel": "String",
  "riskEventStatus": "String",
  "closedDateTime": "2016-12-31T23:59:27.3956276+03:00",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.impossibletravelriskevent"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1245

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
```

