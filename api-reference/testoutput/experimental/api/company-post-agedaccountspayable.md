---
title: "Add agedAccountsPayable"
description: "Add agedAccountsPayable by posting to the agedAccountsPayable collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add agedAccountsPayable

Namespace: microsoft.graph

Add agedAccountsPayable by posting to the agedAccountsPayable collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /financials/companies/{companyId}/agedAccountsPayable/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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
If successful, this method returns a `201 Created` response code and a [agedAccountsPayable](../resources/agedaccountspayable.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_agedaccountspayable_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/financials/companies/{companyId}/agedAccountsPayable
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
  "truncated": true,
  "@odata.type": "microsoft.graph.agedaccountspayable"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 433

{
  "@odata.type": "#microsoft.graph.agedAccountsPayable",
  "id": "ed338a54-8a54-ed33-548a-33ed548a33ed",
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

