---
title: "reportRoot: getMailboxUsageDetail"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# getMailboxUsageDetail

Namespace: microsoft.graph

**TODO: Add Description**

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
GET /reports/getMailboxUsageDetail
GET /print/reports/{reportRootId}/getMailboxUsageDetail
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Parameter|Type|Description|
|:---|:---|:---|
|period|String|**TODO: Add Description**|



## Response
If successful, this function returns a `200 OK` response code and a [mailboxUsageDetail](../resources/mailboxusagedetail.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='parameterValue')
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.mailboxusagedetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mailboxUsageDetail",
      "id": "d4a8528f-528f-d4a8-8f52-a8d48f52a8d4",
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
  ]
}
```

