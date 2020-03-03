---
title: "List mailboxUsageDetails"
description: "List properties and relationships of the mailboxUsageDetail objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List mailboxUsageDetails

List properties and relationships of the [mailboxUsageDetail](../resources/mailboxusagedetail.md) objects.

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
GET ** Collection URI for microsoft.graph.mailboxUsageDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [mailboxUsageDetail](../resources/mailboxusagedetail.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_mailboxusagedetail"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.mailboxUsageDetail not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.mailboxusagedetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 697

{
  "value": [
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
  ]
}
```

