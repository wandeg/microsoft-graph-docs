---
title: "Get mailboxUsageDetail"
description: "Read properties and relationships of the mailboxUsageDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get mailboxUsageDetail

Namespace: microsoft.graph

Read properties and relationships of the [mailboxUsageDetail](../resources/mailboxusagedetail.md) object.

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
GET ** Entity URI for microsoft.graph.mailboxUsageDetail not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [mailboxUsageDetail](../resources/mailboxusagedetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_mailboxusagedetail"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.mailboxUsageDetail not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageDetail"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 649

{
  "value": {
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
}
```

