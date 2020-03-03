---
title: "Get mailboxUsageMailboxCounts"
description: "Read properties and relationships of the mailboxUsageMailboxCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get mailboxUsageMailboxCounts

Namespace: microsoft.graph

Read properties and relationships of the [mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md) object.

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
GET ** Entity URI for microsoft.graph.mailboxUsageMailboxCounts not found
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
If successful, this method returns a `200 OK` response code and [mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_mailboxusagemailboxcounts"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.mailboxUsageMailboxCounts not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageMailboxCounts"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "value": {
    "@odata.type": "#microsoft.graph.mailboxUsageMailboxCounts",
    "id": "b2fe3ac9-3ac9-b2fe-c93a-feb2c93afeb2",
    "reportRefreshDate": "Date",
    "total": 5,
    "active": 6,
    "reportDate": "Date",
    "reportPeriod": "Report Period value"
  }
}
```

