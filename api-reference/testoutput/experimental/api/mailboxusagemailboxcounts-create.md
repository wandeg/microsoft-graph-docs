---
title: "Create mailboxUsageMailboxCounts"
description: "Create a new mailboxUsageMailboxCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create mailboxUsageMailboxCounts

Namespace: microsoft.graph

Create a new [mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md) object.

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
POST ** Collection URI for microsoft.graph.mailboxUsageMailboxCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md) object.

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
If successful, this method returns a `201 Created` response code and a [mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_mailboxusagemailboxcounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.mailboxUsageMailboxCounts not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxusagemailboxcounts"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 246

{
  "@odata.type": "#microsoft.graph.mailboxUsageMailboxCounts",
  "id": "b2fe3ac9-3ac9-b2fe-c93a-feb2c93afeb2",
  "reportRefreshDate": "Date",
  "total": 5,
  "active": 6,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

