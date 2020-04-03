---
title: "Add generalLedgerEntries"
description: "Add generalLedgerEntries by posting to the generalLedgerEntries collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add generalLedgerEntries

Namespace: microsoft.graph

Add generalLedgerEntries by posting to the generalLedgerEntries collection.

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
POST /financials/companies/{companyId}/generalLedgerEntries/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [generalLedgerEntry](../resources/generalledgerentry.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_generalledgerentry_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/generalLedgerEntries
Content-type: application/json
Content-length: 364

{
  "@odata.type": "#microsoft.graph.generalLedgerEntry",
  "postingDate": "Date",
  "documentNumber": "Document Number value",
  "documentType": "Document Type value",
  "accountId": "7085e644-e644-7085-44e6-857044e68570",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.generalledgerentry"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 477

{
  "@odata.type": "#microsoft.graph.generalLedgerEntry",
  "id": "8da02d02-2d02-8da0-022d-a08d022da08d",
  "postingDate": "Date",
  "documentNumber": "Document Number value",
  "documentType": "Document Type value",
  "accountId": "7085e644-e644-7085-44e6-857044e68570",
  "accountNumber": "Account Number value",
  "description": "Description value",
  "debitAmount": "4.2",
  "creditAmount": "4.2",
  "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00"
}
```

