---
title: "Get mailboxUsageQuotaStatusMailboxCounts"
description: "Read properties and relationships of the mailboxUsageQuotaStatusMailboxCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get mailboxUsageQuotaStatusMailboxCounts

Namespace: microsoft.graph

Read properties and relationships of the [mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md) object.

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
GET ** Entity URI for microsoft.graph.mailboxUsageQuotaStatusMailboxCounts not found
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
If successful, this method returns a `200 OK` response code and [mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_mailboxusagequotastatusmailboxcounts"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.mailboxUsageQuotaStatusMailboxCounts not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageQuotaStatusMailboxCounts"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 390

{
  "value": {
    "@odata.type": "#microsoft.graph.mailboxUsageQuotaStatusMailboxCounts",
    "id": "cec16fca-6fca-cec1-ca6f-c1ceca6fc1ce",
    "reportRefreshDate": "Date",
    "underLimit": 10,
    "warningIssued": 13,
    "sendProhibited": 14,
    "sendReceiveProhibited": 5,
    "indeterminate": 13,
    "reportDate": "Date",
    "reportPeriod": "Report Period value"
  }
}
```

