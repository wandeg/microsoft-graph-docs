---
title: "getMailboxUsageQuotaStatusMailboxCounts"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getMailboxUsageQuotaStatusMailboxCounts

Namespace: microsoft.graph



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
GET /reports/getMailboxUsageQuotaStatusMailboxCounts
GET /print/reports/{reportRootId}/getMailboxUsageQuotaStatusMailboxCounts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|period|String||



## Response
If successful, this function returns a `200 OK` response code and a [mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageQuotaStatusMailboxCounts(period='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.mailboxusagequotastatusmailboxcounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 424

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mailboxUsageQuotaStatusMailboxCounts",
      "id": "9416a468-a468-9416-68a4-169468a41694",
      "reportRefreshDate": "Date",
      "underLimit": 10,
      "warningIssued": 13,
      "sendProhibited": 14,
      "sendReceiveProhibited": 5,
      "indeterminate": 13,
      "reportDate": "Date",
      "reportPeriod": "Report Period value"
    }
  ]
}
```

