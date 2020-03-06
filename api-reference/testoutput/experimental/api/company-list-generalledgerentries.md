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
|Header|Value|
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
GET https://graph.microsoft.com/localtest/financials/companies/{companyId}/generalLedgerEntries
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
      "id": "e228ae17-ae17-e228-17ae-28e217ae28e2",
      "postingDate": "Date",
      "documentNumber": "Document Number value",
      "documentType": "Document Type value",
      "accountId": "16975858-5858-1697-5858-971658589716",
      "accountNumber": "Account Number value",
      "description": "Description value",
      "debitAmount": "4.2",
      "creditAmount": "4.2",
      "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00"
    }
  ]
}
```

