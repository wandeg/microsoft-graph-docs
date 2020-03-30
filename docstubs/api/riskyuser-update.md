---
title: "Update riskyUser"
description: "Update the properties of a riskyUser object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update riskyUser

Namespace: microsoft.graph

Update the properties of a [riskyUser](../resources/riskyuser.md) object.

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
PATCH /riskyUsers/{riskyUsersId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [riskyUser](../resources/riskyuser.md) object.

The following table shows the properties that are required when you create the [riskyUser](../resources/riskyuser.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isDeleted|Boolean||
|isGuest|Boolean||
|isProcessing|Boolean||
|riskLastUpdatedDateTime|DateTimeOffset||
|riskLevel|Enumeration| Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|Enumeration| Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|riskDetail|Enumeration| Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|userDisplayName|String||
|userPrincipalName|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [riskyUser](../resources/riskyuser.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_riskyuser"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/riskyUsers/{riskyUsersId}
Content-type: application/json
Content-length: 366

{
  "@odata.type": "#microsoft.graph.riskyUser",
  "isDeleted": true,
  "isGuest": true,
  "isProcessing": true,
  "riskLastUpdatedDateTime": "2017-01-01T00:01:08.3483547+00:00",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value"
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
Content-Length: 415

{
  "@odata.type": "#microsoft.graph.riskyUser",
  "id": "bd714188-4188-bd71-8841-71bd884171bd",
  "isDeleted": true,
  "isGuest": true,
  "isProcessing": true,
  "riskLastUpdatedDateTime": "2017-01-01T00:01:08.3483547+00:00",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value"
}
```

