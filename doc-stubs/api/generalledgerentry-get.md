---
title: "Get generalLedgerEntry"
description: "Read the properties and relationships of a generalLedgerEntry object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get generalLedgerEntry

Namespace: microsoft.graph

Read the properties and relationships of a [generalLedgerEntry](../resources/generalledgerentry.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

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
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [generalLedgerEntry](../resources/generalledgerentry.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_generalledgerentry"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/generalLedgerEntries/{generalLedgerEntryId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.generalLedgerEntry"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.generalLedgerEntry",
    "id": "a0692c8f-2c8f-a069-8f2c-69a08f2c69a0",
    "postingDate": "Date",
    "documentNumber": "String",
    "documentType": "String",
    "accountId": "Guid",
    "accountNumber": "String",
    "description": "String",
    "debitAmount": "Decimal",
    "creditAmount": "Decimal",
    "lastModifiedDateTime": "String (timestamp)"
  }
}
```

