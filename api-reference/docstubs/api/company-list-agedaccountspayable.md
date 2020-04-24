---
title: "List agedAccountsPayable"
description: "Get the agedAccountsPayables from the agedAccountsPayable navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List agedAccountsPayable

Namespace: microsoft.graph

Get the agedAccountsPayables from the agedAccountsPayable navigation property.

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
GET /financials/companies/{companyId}/agedAccountsPayable
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
If successful, this method returns a `200 OK` response code and a collection of [agedAccountsPayable](../resources/agedaccountspayable.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_agedaccountspayable"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/agedAccountsPayable
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.agedaccountspayable)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.agedAccountsPayable",
      "id": "0a123154-3154-0a12-5431-120a5431120a",
      "vendorNumber": "Vendor Number value",
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

