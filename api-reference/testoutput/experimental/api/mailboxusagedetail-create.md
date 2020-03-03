---
title: "Create mailboxUsageDetail"
description: "Create a new mailboxUsageDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create mailboxUsageDetail

Create a new [mailboxUsageDetail](../resources/mailboxusagedetail.md) object.

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
POST ** Collection URI for microsoft.graph.mailboxUsageDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the mailboxUsageDetail object.

The following table shows the properties that are required when you create the mailboxUsageDetail.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|userPrincipalName|String||
|displayName|String||
|isDeleted|Boolean||
|deletedDate|Date||
|createdDate|Date||
|lastActivityDate|Date||
|itemCount|Int64||
|storageUsedInBytes|Int64||
|deletedItemCount|Int64||
|deletedItemSizeInBytes|Int64||
|issueWarningQuotaInBytes|Int64||
|prohibitSendQuotaInBytes|Int64||
|prohibitSendReceiveQuotaInBytes|Int64||
|reportPeriod|String||



## Response
If successful, this method returns a `201 Created` response code and a [mailboxUsageDetail](../resources/mailboxusagedetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_mailboxusagedetail_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.mailboxUsageDetail not found
Content-type: application/json
Content-length: 547

{
  "@odata.type": "#microsoft.graph.mailboxUsageDetail",
  "reportRefreshDate": "Date",
  "userPrincipalName": "User Principal Name value",
  "displayName": "Display Name value",
  "isDeleted": true,
  "deletedDate": "Date",
  "createdDate": "Date",
  "lastActivityDate": "Date",
  "itemCount": 9,
  "storageUsedInBytes": 2,
  "deletedItemCount": 0,
  "deletedItemSizeInBytes": 6,
  "issueWarningQuotaInBytes": 8,
  "prohibitSendQuotaInBytes": 8,
  "prohibitSendReceiveQuotaInBytes": 15,
  "reportPeriod": "Report Period value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxusagedetail"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 596

{
  "@odata.type": "#microsoft.graph.mailboxUsageDetail",
  "id": "77bac344-c344-77ba-44c3-ba7744c3ba77",
  "reportRefreshDate": "Date",
  "userPrincipalName": "User Principal Name value",
  "displayName": "Display Name value",
  "isDeleted": true,
  "deletedDate": "Date",
  "createdDate": "Date",
  "lastActivityDate": "Date",
  "itemCount": 9,
  "storageUsedInBytes": 2,
  "deletedItemCount": 0,
  "deletedItemSizeInBytes": 6,
  "issueWarningQuotaInBytes": 8,
  "prohibitSendQuotaInBytes": 8,
  "prohibitSendReceiveQuotaInBytes": 15,
  "reportPeriod": "Report Period value"
}
```

