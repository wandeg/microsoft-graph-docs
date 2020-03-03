---
title: "Get generalLedgerEntry"
description: "Read properties and relationships of the generalLedgerEntry object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get generalLedgerEntry

Namespace: microsoft.graph

Read properties and relationships of the [generalLedgerEntry](../resources/generalledgerentry.md) object.

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
GET /financials/companies/{companyId}/generalLedgerEntries/{generalLedgerEntryId}
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
If successful, this method returns a `200 OK` response code and [generalLedgerEntry](../resources/generalledgerentry.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_generalledgerentry"
}
-->
``` http
GET https://graph.microsoft.com/localtest/financials/companies/{companyId}/generalLedgerEntries/{generalLedgerEntryId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.generalLedgerEntry"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 518

{
  "value": {
    "@odata.type": "#microsoft.graph.generalLedgerEntry",
    "id": "aa869a60-9a60-aa86-609a-86aa609a86aa",
    "postingDate": "Date",
    "documentNumber": "Document Number value",
    "documentType": "Document Type value",
    "accountId": "95554513-4513-9555-1345-559513455595",
    "accountNumber": "Account Number value",
    "description": "Description value",
    "debitAmount": "4.2",
    "creditAmount": "4.2",
    "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00"
  }
}
```

