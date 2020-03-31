---
title: "Update generalLedgerEntry"
description: "Update the properties of a generalLedgerEntry object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update generalLedgerEntry

Namespace: microsoft.graph

Update the properties of a [generalLedgerEntry](../resources/generalledgerentry.md) object.

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
PATCH /financials/companies/{companyId}/generalLedgerEntries/{generalLedgerEntryId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [generalLedgerEntry](../resources/generalledgerentry.md) object.

The following table shows the properties that are required when you create the [generalLedgerEntry](../resources/generalledgerentry.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|postingDate|Date||
|documentNumber|String||
|documentType|String||
|accountId|Guid||
|accountNumber|String||
|description|String||
|debitAmount|Decimal||
|creditAmount|Decimal||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [generalLedgerEntry](../resources/generalledgerentry.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_generalledgerentry"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/generalLedgerEntries/{generalLedgerEntryId}
Content-type: application/json
Content-length: 364

{
  "@odata.type": "#microsoft.graph.generalLedgerEntry",
  "postingDate": "Date",
  "documentNumber": "Document Number value",
  "documentType": "Document Type value",
  "accountId": "ca9f694c-694c-ca9f-4c69-9fca4c699fca",
  "accountNumber": "Account Number value",
  "description": "Description value",
  "debitAmount": "4.2",
  "creditAmount": "4.2"
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
Content-Length: 477

{
  "@odata.type": "#microsoft.graph.generalLedgerEntry",
  "id": "c1d91c7e-1c7e-c1d9-7e1c-d9c17e1cd9c1",
  "postingDate": "Date",
  "documentNumber": "Document Number value",
  "documentType": "Document Type value",
  "accountId": "ca9f694c-694c-ca9f-4c69-9fca4c699fca",
  "accountNumber": "Account Number value",
  "description": "Description value",
  "debitAmount": "4.2",
  "creditAmount": "4.2",
  "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00"
}
```

