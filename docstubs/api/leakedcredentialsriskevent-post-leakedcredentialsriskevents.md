---
title: "Create leakedCredentialsRiskEvent"
description: "Create a new leakedCredentialsRiskEvent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create leakedCredentialsRiskEvent

Namespace: microsoft.graph

Create a new [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object.

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
POST /leakedCredentialsRiskEvents
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object.

The following table shows the properties that are required when you create the [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md).

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



## Response
If successful, this method returns a `201 Created` response code and a [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_leakedcredentialsriskevent_from_leakedcredentialsriskevents"
}
-->
``` http
POST https://graph.microsoft.com/beta/leakedCredentialsRiskEvents
Content-type: application/json
Content-length: 421

{
  "@odata.type": "#microsoft.graph.leakedCredentialsRiskEvent",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "riskEventDateTime": "2017-01-01T00:02:40.748803+00:00",
  "riskEventType": "Risk Event Type value",
  "riskLevel": "String",
  "riskEventStatus": "String",
  "closedDateTime": "2017-01-01T00:01:42.8390447+00:00",
  "userId": "User Id value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.leakedcredentialsriskevent"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.leakedCredentialsRiskEvent",
  "id": "646968b9-68b9-6469-b968-6964b9686964",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "riskEventDateTime": "2017-01-01T00:02:40.748803+00:00",
  "riskEventType": "Risk Event Type value",
  "riskLevel": "String",
  "riskEventStatus": "String",
  "closedDateTime": "2017-01-01T00:01:42.8390447+00:00",
  "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
  "userId": "User Id value"
}
```

