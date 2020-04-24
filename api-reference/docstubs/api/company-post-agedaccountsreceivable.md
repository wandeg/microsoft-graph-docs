---
title: "Create agedAccountsReceivable"
description: "Create a new agedAccountsReceivable object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create agedAccountsReceivable

Namespace: microsoft.graph

Create a new agedAccountsReceivable object.

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
POST /financials/companies/{companyId}/agedAccountsReceivable
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [agedAccountsReceivable](../resources/agedaccountsreceivable.md) object.

The following table shows the properties that are required when you create the [agedAccountsReceivable](../resources/agedaccountsreceivable.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|customerNumber|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|currencyCode|String|**TODO: Add Description**|
|balanceDue|Decimal|**TODO: Add Description**|
|currentAmount|Decimal|**TODO: Add Description**|
|period1Amount|Decimal|**TODO: Add Description**|
|period2Amount|Decimal|**TODO: Add Description**|
|period3Amount|Decimal|**TODO: Add Description**|
|agedAsOfDate|Date|**TODO: Add Description**|
|periodLengthFilter|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [agedAccountsReceivable](../resources/agedaccountsreceivable.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_agedaccountsreceivable_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/agedAccountsReceivable
Content-Type: application/json
Content-length: 391

{
  "@odata.type": "#microsoft.graph.agedAccountsReceivable",
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
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agedaccountsreceivable"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
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
```

