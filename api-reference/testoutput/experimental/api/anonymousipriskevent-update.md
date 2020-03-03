---
title: "Update anonymousIpRiskEvent"
description: "Update the properties of a anonymousIpRiskEvent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update anonymousIpRiskEvent

Update the properties of a [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object.

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
PATCH /anonymousIpRiskEvents/{anonymousIpRiskEventsId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [anonymousIpRiskEvent](../resources/anonymousIpRiskEvent.md) object.

The following table shows the properties that are required when you create the [anonymousIpRiskEvent](../resources/anonymousipriskevent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userDisplayName|String| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md)|
|userPrincipalName|String| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md)|
|riskEventDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md)|
|riskEventType|String| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md)|
|riskLevel|Enumeration| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskEventStatus|Enumeration| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md). Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|closedDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md)|
|createdDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md)|
|userId|String| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md)|
|location|[signInLocation](../resources/signInLocation.md)| Inherited from [locatedRiskEvent](../resources/locatedRiskEvent.md)|
|ipAddress|String| Inherited from [locatedRiskEvent](../resources/locatedRiskEvent.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_anonymousipriskevent"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/anonymousIpRiskEvents/{anonymousIpRiskEventsId}
Content-type: application/json
Content-length: 811

{
  "@odata.type": "#microsoft.graph.anonymousIpRiskEvent",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "riskEventDateTime": "2017-01-01T00:01:00.7804275+03:00",
  "riskEventType": "Risk Event Type value",
  "riskLevel": "String",
  "riskEventStatus": "String",
  "closedDateTime": "2017-01-01T00:01:30.8768135+03:00",
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
Content-Length: 919

{
  "@odata.type": "#microsoft.graph.anonymousIpRiskEvent",
  "id": "c4d06eb0-6eb0-c4d0-b06e-d0c4b06ed0c4",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "riskEventDateTime": "2017-01-01T00:01:00.7804275+03:00",
  "riskEventType": "Risk Event Type value",
  "riskLevel": "String",
  "riskEventStatus": "String",
  "closedDateTime": "2017-01-01T00:01:30.8768135+03:00",
  "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
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

