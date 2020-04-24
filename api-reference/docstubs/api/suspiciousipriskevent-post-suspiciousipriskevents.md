---
title: "Create suspiciousIpRiskEvent"
description: "Create a new suspiciousIpRiskEvent object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create suspiciousIpRiskEvent

Namespace: microsoft.graph

Create a new [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) object.

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
POST /suspiciousIpRiskEvents
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) object.

The following table shows the properties that are required when you create the [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|userDisplayName|String|**TODO: Add Description** Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|userPrincipalName|String|**TODO: Add Description** Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|riskEventDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|riskEventType|String|**TODO: Add Description** Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|riskLevel|riskLevel|**TODO: Add Description** Inherited from [identityRiskEvent](../resources/identityriskevent.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskEventStatus|riskEventStatus|**TODO: Add Description** Inherited from [identityRiskEvent](../resources/identityriskevent.md). Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|closedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|userId|String|**TODO: Add Description** Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|location|[signInLocation](../resources/signinlocation.md)|**TODO: Add Description** Inherited from [locatedRiskEvent](../resources/locatedriskevent.md)|
|ipAddress|String|**TODO: Add Description** Inherited from [locatedRiskEvent](../resources/locatedriskevent.md)|



## Response
If successful, this method returns a `201 Created` response code and a [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_suspiciousipriskevent_from_suspiciousipriskevents"
}
-->
``` http
POST https://graph.microsoft.com/beta/suspiciousIpRiskEvents
Content-Type: application/json
Content-length: 812

{
  "@odata.type": "#microsoft.graph.suspiciousIpRiskEvent",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "riskEventDateTime": "2017-01-01T00:02:03.6171597+03:00",
  "riskEventType": "Risk Event Type value",
  "riskLevel": "String",
  "riskEventStatus": "String",
  "closedDateTime": "2016-12-31T23:58:06.1799456+03:00",
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.suspiciousipriskevent"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.suspiciousIpRiskEvent",
  "id": "4bb10f04-0f04-4bb1-040f-b14b040fb14b",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "riskEventDateTime": "2017-01-01T00:02:03.6171597+03:00",
  "riskEventType": "Risk Event Type value",
  "riskLevel": "String",
  "riskEventStatus": "String",
  "closedDateTime": "2016-12-31T23:58:06.1799456+03:00",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
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

