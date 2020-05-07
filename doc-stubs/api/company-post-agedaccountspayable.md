---
title: "Create agedAccountsPayable"
description: "Create a new agedAccountsPayable object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create agedAccountsPayable

Namespace: microsoft.graph

Create a new agedAccountsPayable object.

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
POST /financials/companies/{companyId}/agedAccountsPayable
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [agedAccountsPayable](../resources/agedaccountspayable.md) object.

The following table shows the properties that are required when you create the [agedAccountsPayable](../resources/agedaccountspayable.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|vendorNumber|String|**TODO: Add Description**|
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

If successful, this method returns a `201 Created` response code and an [agedAccountsPayable](../resources/agedaccountspayable.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_agedaccountspayable_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/agedAccountsPayable
Content-Type: application/json
Content-length: 354

{
  "@odata.type": "#microsoft.graph.agedAccountsPayable",
  "vendorNumber": "String",
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
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agedaccountspayable"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.agedAccountsPayable",
  "id": "8963f23f-f23f-8963-3ff2-63893ff26389",
  "vendorNumber": "String",
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
```

