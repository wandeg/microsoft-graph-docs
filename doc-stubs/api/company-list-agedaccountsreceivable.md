---
title: "List agedAccountsReceivable"
description: "Get the agedAccountsReceivables from the agedAccountsReceivable navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List agedAccountsReceivable

Namespace: microsoft.graph

Get the agedAccountsReceivables from the agedAccountsReceivable navigation property.

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
GET /financials/companies/{companyId}/agedAccountsReceivable
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

If successful, this method returns a `200 OK` response code and a collection of [agedAccountsReceivable](../resources/agedaccountsreceivable.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_agedaccountsreceivable"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/agedAccountsReceivable
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.agedaccountsreceivable)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.agedAccountsReceivable",
      "id": "699a54ab-54ab-699a-ab54-9a69ab549a69",
      "customerNumber": "String",
      "name": "String",
      "currencyCode": "String",
      "balanceDue": "Decimal",
      "currentAmount": "Decimal",
      "period1Amount": "Decimal",
      "period2Amount": "Decimal",
      "period3Amount": "Decimal",
      "agedAsOfDate": "Date",
      "periodLengthFilter": "String"
    }
  ]
}
```

