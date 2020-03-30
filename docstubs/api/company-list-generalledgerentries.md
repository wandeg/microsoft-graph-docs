---
title: "List generalLedgerEntries"
description: "Get the generalLedgerEntries from the generalLedgerEntries navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List generalLedgerEntries

Namespace: microsoft.graph

Get the generalLedgerEntries from the generalLedgerEntries navigation property.

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
GET /financials/companies/{companyId}/generalLedgerEntries
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
If successful, this method returns a `200 OK` response code and a collection of [generalLedgerEntry](../resources/generalledgerentry.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_generalledgerentry"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/generalLedgerEntries
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.generalledgerentry)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 554

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.generalLedgerEntry",
      "id": "6a1af1a0-f1a0-6a1a-a0f1-1a6aa0f11a6a",
      "postingDate": "Date",
      "documentNumber": "Document Number value",
      "documentType": "Document Type value",
      "accountId": "ec2602f3-02f3-ec26-f302-26ecf30226ec",
      "accountNumber": "Account Number value",
      "description": "Description value",
      "debitAmount": "4.2",
      "creditAmount": "4.2",
      "lastModifiedDateTime": "2017-01-01T00:02:50.3839766+00:00"
    }
  ]
}
```

