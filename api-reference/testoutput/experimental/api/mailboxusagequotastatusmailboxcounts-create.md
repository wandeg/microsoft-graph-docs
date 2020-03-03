---
title: "Create mailboxUsageQuotaStatusMailboxCounts"
description: "Create a new mailboxUsageQuotaStatusMailboxCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create mailboxUsageQuotaStatusMailboxCounts

Create a new [mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md) object.

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
POST ** Collection URI for microsoft.graph.mailboxUsageQuotaStatusMailboxCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the mailboxUsageQuotaStatusMailboxCounts object.

The following table shows the properties that are required when you create the mailboxUsageQuotaStatusMailboxCounts.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|underLimit|Int64||
|warningIssued|Int64||
|sendProhibited|Int64||
|sendReceiveProhibited|Int64||
|indeterminate|Int64||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `201 Created` response code and a [mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_mailboxusagequotastatusmailboxcounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.mailboxUsageQuotaStatusMailboxCounts not found
Content-type: application/json
Content-length: 302

{
  "@odata.type": "#microsoft.graph.mailboxUsageQuotaStatusMailboxCounts",
  "reportRefreshDate": "Date",
  "underLimit": 10,
  "warningIssued": 13,
  "sendProhibited": 14,
  "sendReceiveProhibited": 5,
  "indeterminate": 13,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxusagequotastatusmailboxcounts"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 351

{
  "@odata.type": "#microsoft.graph.mailboxUsageQuotaStatusMailboxCounts",
  "id": "1d2716ae-16ae-1d27-ae16-271dae16271d",
  "reportRefreshDate": "Date",
  "underLimit": 10,
  "warningIssued": 13,
  "sendProhibited": 14,
  "sendReceiveProhibited": 5,
  "indeterminate": 13,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

