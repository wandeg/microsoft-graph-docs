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
|Authorization|Bearer {token}. Required|

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
      "id": "18913568-3568-1891-6835-911868359118",
      "customerNumber": "Customer Number value",
      "name": "Name value",
      "currencyCode": "Currency Code value",
      "balanceDue": "4.2",
      "currentAmount": "4.2",
      "period1Amount": "4.2",
      "period2Amount": "4.2",
      "period3Amount": "4.2",
      "agedAsOfDate": "Date",
      "periodLengthFilter": "Period Length Filter value"
    }
  ]
}
```

