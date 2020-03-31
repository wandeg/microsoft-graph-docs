---
title: "Update agedAccountsPayable"
description: "Update the properties of a agedAccountsPayable object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update agedAccountsPayable

Namespace: microsoft.graph

Update the properties of a [agedAccountsPayable](../resources/agedaccountspayable.md) object.

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
PATCH /financials/companies/{companyId}/agedAccountsPayable/{agedAccountsPayableId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [agedAccountsPayable](../resources/agedaccountspayable.md) object.

The following table shows the properties that are required when you create the [agedAccountsPayable](../resources/agedaccountspayable.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|vendorNumber|String||
|name|String||
|currencyCode|String||
|balanceDue|Decimal||
|currentAmount|Decimal||
|period1Amount|Decimal||
|period2Amount|Decimal||
|period3Amount|Decimal||
|agedAsOfDate|Date||
|periodLengthFilter|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [agedAccountsPayable](../resources/agedaccountspayable.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_agedaccountspayable"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/agedAccountsPayable/{agedAccountsPayableId}
Content-type: application/json
Content-length: 384

{
  "@odata.type": "#microsoft.graph.agedAccountsPayable",
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
Content-Length: 433

{
  "@odata.type": "#microsoft.graph.agedAccountsPayable",
  "id": "61da2f63-2f63-61da-632f-da61632fda61",
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
```

