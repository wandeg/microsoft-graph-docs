---
title: "Update mailboxUsageMailboxCounts"
description: "Update the properties of a mailboxUsageMailboxCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update mailboxUsageMailboxCounts

Update the properties of a [mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md) object.

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
PATCH ** Entity URI for microsoft.graph.mailboxUsageMailboxCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [mailboxUsageMailboxCounts](../resources/mailboxUsageMailboxCounts.md) object.

The following table shows the properties that are required when you create the [mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|total|Int64||
|active|Int64||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_mailboxusagemailboxcounts"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.mailboxUsageMailboxCounts not found
Content-type: application/json
Content-length: 197

{
  "@odata.type": "#microsoft.graph.mailboxUsageMailboxCounts",
  "reportRefreshDate": "Date",
  "total": 5,
  "active": 6,
  "reportDate": "Date",
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
Content-Length: 246

{
  "@odata.type": "#microsoft.graph.mailboxUsageMailboxCounts",
  "id": "038e5c62-5c62-038e-625c-8e03625c8e03",
  "reportRefreshDate": "Date",
  "total": 5,
  "active": 6,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

