---
title: "Create history"
description: "Create a new history object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create history

Namespace: microsoft.graph

Create a new history object.

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
POST /riskyUsers/{riskyUsersId}/history
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.

The following table shows the properties that are required when you create the [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isDeleted|Boolean|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md)|
|isGuest|Boolean|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md)|
|isProcessing|Boolean|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md)|
|riskLastUpdatedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md)|
|riskLevel|riskLevel|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md). Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|riskDetail|riskDetail|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md). Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|userDisplayName|String|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md)|
|userPrincipalName|String|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md)|
|userId|String|**TODO: Add Description**|
|initiatedBy|String|**TODO: Add Description**|
|activity|[riskUserActivity](../resources/riskuseractivity.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_riskyuserhistoryitem_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/riskyUsers/{riskyUsersId}/history
Content-Type: application/json
Content-length: 660

{
  "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
  "isDeleted": true,
  "isGuest": true,
  "isProcessing": true,
  "riskLastUpdatedDateTime": "2016-12-31T23:58:33.1152347+03:00",
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
    "riskEventTypes": [
      "Risk Event Types value"
    ],
    "detail": "String"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyuserhistoryitem"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
  "id": "1a608df0-8df0-1a60-f08d-601af08d601a",
  "isDeleted": true,
  "isGuest": true,
  "isProcessing": true,
  "riskLastUpdatedDateTime": "2016-12-31T23:58:33.1152347+03:00",
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
    "riskEventTypes": [
      "Risk Event Types value"
    ],
    "detail": "String"
  }
}
```

