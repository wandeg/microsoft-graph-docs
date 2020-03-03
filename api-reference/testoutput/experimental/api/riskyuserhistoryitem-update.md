---
title: "Update riskyUserHistoryItem"
description: "Update the properties of a riskyUserHistoryItem object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update riskyUserHistoryItem

Update the properties of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.

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
PATCH /riskyUsers/{riskyUsersId}/history/{riskyUserHistoryItemId}
PATCH /riskyUsers/{riskyUsersId}/history/{riskyUserHistoryItemId}/history/{riskyUserHistoryItemId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [riskyUserHistoryItem](../resources/riskyUserHistoryItem.md) object.

The following table shows the properties that are required when you create the [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isDeleted|Boolean| Inherited from [riskyUser](../resources/riskyUser.md)|
|isGuest|Boolean| Inherited from [riskyUser](../resources/riskyUser.md)|
|isProcessing|Boolean| Inherited from [riskyUser](../resources/riskyUser.md)|
|riskLastUpdatedDateTime|DateTimeOffset| Inherited from [riskyUser](../resources/riskyUser.md)|
|riskLevel|Enumeration| Inherited from [riskyUser](../resources/riskyUser.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|Enumeration| Inherited from [riskyUser](../resources/riskyUser.md). Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|riskDetail|Enumeration| Inherited from [riskyUser](../resources/riskyUser.md). Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|userDisplayName|String| Inherited from [riskyUser](../resources/riskyUser.md)|
|userPrincipalName|String| Inherited from [riskyUser](../resources/riskyUser.md)|
|userId|String||
|initiatedBy|String||
|activity|[riskUserActivity](../resources/riskUserActivity.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_riskyuserhistoryitem"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/riskyUsers/{riskyUsersId}/history/{riskyUserHistoryItemId}
Content-type: application/json
Content-length: 595

{
  "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
  "isDeleted": true,
  "isGuest": true,
  "isProcessing": true,
  "riskLastUpdatedDateTime": "2016-12-31T23:56:32.9362095+03:00",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "userId": "User Id value",
  "initiatedBy": "Initiated By value",
  "activity": {
    "@odata.type": "microsoft.graph.riskUserActivity",
    "eventTypes": [
      "String"
    ],
    "detail": "String"
  }
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
Content-Length: 644

{
  "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
  "id": "7e9fd1ac-d1ac-7e9f-acd1-9f7eacd19f7e",
  "isDeleted": true,
  "isGuest": true,
  "isProcessing": true,
  "riskLastUpdatedDateTime": "2016-12-31T23:56:32.9362095+03:00",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "userId": "User Id value",
  "initiatedBy": "Initiated By value",
  "activity": {
    "@odata.type": "microsoft.graph.riskUserActivity",
    "eventTypes": [
      "String"
    ],
    "detail": "String"
  }
}
```

