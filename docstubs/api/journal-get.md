---
title: "Get journal"
description: "Read properties and relationships of the journal object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get journal

Namespace: microsoft.graph

Read properties and relationships of the [journal](../resources/journal.md) object.

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
GET /financials/companies/{companyId}/journals/{journalId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [journal](../resources/journal.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_journal"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/journals/{journalId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.journal"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 388

{
  "value": {
    "@odata.type": "#microsoft.graph.journal",
    "id": "06bfc720-c720-06bf-20c7-bf0620c7bf06",
    "code": "Code value",
    "displayName": "Display Name value",
    "lastModifiedDateTime": "2017-01-01T00:01:52.9217945+03:00",
    "balancingAccountId": "6cdf2014-2014-6cdf-1420-df6c1420df6c",
    "balancingAccountNumber": "Balancing Account Number value"
  }
}
```

