---
title: "Add history"
description: "Add history by posting to the history collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add history

Namespace: microsoft.graph

Add history by posting to the history collection.

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
POST /riskyUsers/{riskyUsersId}/history/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.

The following table shows the properties that are required when you create the [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isDeleted|Boolean| Inherited from [riskyUser](../resources/riskyuser.md)|
|isGuest|Boolean| Inherited from [riskyUser](../resources/riskyuser.md)|
|isProcessing|Boolean| Inherited from [riskyUser](../resources/riskyuser.md)|
|riskLastUpdatedDateTime|DateTimeOffset| Inherited from [riskyUser](../resources/riskyuser.md)|
|riskLevel|Enumeration| Inherited from [riskyUser](../resources/riskyuser.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|Enumeration| Inherited from [riskyUser](../resources/riskyuser.md). Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|riskDetail|Enumeration| Inherited from [riskyUser](../resources/riskyuser.md). Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|userDisplayName|String| Inherited from [riskyUser](../resources/riskyuser.md)|
|userPrincipalName|String| Inherited from [riskyUser](../resources/riskyuser.md)|
|userId|String||
|initiatedBy|String||
|activity|[riskUserActivity](../resources/riskuseractivity.md)||



## Response
If successful, this method returns a `201 Created` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_riskyuserhistoryitem_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/riskyUsers/{riskyUsersId}/history
Content-type: application/json
Content-length: 595

{
  "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
  "isDeleted": true,
  "isGuest": true,
  "isProcessing": true,
  "riskLastUpdatedDateTime": "2017-01-01T00:02:54.3614539+03:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyuserhistoryitem"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 644

{
  "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
  "id": "78955313-5313-7895-1353-957813539578",
  "isDeleted": true,
  "isGuest": true,
  "isProcessing": true,
  "riskLastUpdatedDateTime": "2017-01-01T00:02:54.3614539+03:00",
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

