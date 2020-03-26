---
title: "Update identityRiskEvent"
description: "Update the properties of a identityRiskEvent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update identityRiskEvent

Namespace: microsoft.graph

Update the properties of a [identityRiskEvent](../resources/identityriskevent.md) object.

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
PATCH /identityRiskEvents/{identityRiskEventsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [identityRiskEvent](../resources/identityriskevent.md) object.

The following table shows the properties that are required when you create the [identityRiskEvent](../resources/identityriskevent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userDisplayName|String||
|userPrincipalName|String||
|riskEventDateTime|DateTimeOffset||
|riskEventType|String||
|riskLevel|Enumeration|. Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskEventStatus|Enumeration|. Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|closedDateTime|DateTimeOffset||
|createdDateTime|DateTimeOffset||
|userId|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [identityRiskEvent](../resources/identityriskevent.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_identityriskevent"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityRiskEvents/{identityRiskEventsId}
Content-type: application/json
Content-length: 413

{
  "@odata.type": "#microsoft.graph.identityRiskEvent",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "riskEventDateTime": "2016-12-31T23:58:59.2098574+03:00",
  "riskEventType": "Risk Event Type value",
  "riskLevel": "String",
  "riskEventStatus": "String",
  "closedDateTime": "2016-12-31T23:56:57.8060591+03:00",
  "userId": "User Id value"
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
Content-Length: 521

{
  "@odata.type": "#microsoft.graph.identityRiskEvent",
  "id": "068dbcfe-bcfe-068d-febc-8d06febc8d06",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "riskEventDateTime": "2016-12-31T23:58:59.2098574+03:00",
  "riskEventType": "Risk Event Type value",
  "riskLevel": "String",
  "riskEventStatus": "String",
  "closedDateTime": "2016-12-31T23:56:57.8060591+03:00",
  "createdDateTime": "2017-01-01T00:00:37.2865022+03:00",
  "userId": "User Id value"
}
```

