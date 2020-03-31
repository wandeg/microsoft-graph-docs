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

## HTTP request
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
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [generalLedgerEntry](../resources/generalledgerentry.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_generalledgerentry"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/generalLedgerEntries/{generalLedgerEntryId}
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
Content-Length: 517

{
  "value": {
    "@odata.type": "#microsoft.graph.generalLedgerEntry",
    "id": "7326bb67-bb67-7326-67bb-267367bb2673",
    "postingDate": "Date",
    "documentNumber": "Document Number value",
    "documentType": "Document Type value",
    "accountId": "ecadd616-d616-ecad-16d6-adec16d6adec",
    "accountNumber": "Account Number value",
    "description": "Description value",
    "debitAmount": "4.2",
    "creditAmount": "4.2",
    "lastModifiedDateTime": "2017-01-01T00:02:23.471109+03:00"
  }
}
```

