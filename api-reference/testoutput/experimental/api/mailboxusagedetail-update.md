---
title: "Update mailboxUsageDetail"
description: "Update the properties of a mailboxUsageDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update mailboxUsageDetail

Namespace: microsoft.graph

Update the properties of a [mailboxUsageDetail](../resources/mailboxusagedetail.md) object.

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
PATCH ** Entity URI for microsoft.graph.mailboxUsageDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [mailboxUsageDetail](../resources/mailboxusagedetail.md) object.

The following table shows the properties that are required when you create the [mailboxUsageDetail](../resources/mailboxusagedetail.md).

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
If successful, this method returns a `200 OK` response code and an updated [mailboxUsageDetail](../resources/mailboxusagedetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_mailboxusagedetail"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.mailboxUsageDetail not found
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 596

{
  "@odata.type": "#microsoft.graph.mailboxUsageDetail",
  "id": "d76f3fbc-3fbc-d76f-bc3f-6fd7bc3f6fd7",
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

