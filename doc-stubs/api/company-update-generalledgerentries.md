---
title: "Update generalLedgerEntries"
description: "Update the properties of a generalLedgerEntries object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update generalLedgerEntries

Namespace: microsoft.graph

Update the properties of a generalLedgerEntries object.

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
PATCH /financials/companies/{companyId}/generalLedgerEntries
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [generalLedgerEntry](../resources/generalledgerentry.md) object.

The following table shows the properties that are required when you create the [generalLedgerEntry](../resources/generalledgerentry.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|postingDate|Date|**TODO: Add Description**|
|documentNumber|String|**TODO: Add Description**|
|documentType|String|**TODO: Add Description**|
|accountId|Guid|**TODO: Add Description**|
|accountNumber|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|debitAmount|Decimal|**TODO: Add Description**|
|creditAmount|Decimal|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [generalLedgerEntry](../resources/generalledgerentry.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_generalledgerentries"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/generalLedgerEntries
Content-Type: application/json
Content-length: 287

{
  "@odata.type": "#microsoft.graph.generalLedgerEntry",
  "postingDate": "Date",
  "documentNumber": "String",
  "documentType": "String",
  "accountId": "Guid",
  "accountNumber": "String",
  "description": "String",
  "debitAmount": "Decimal",
  "creditAmount": "Decimal"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
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
```

