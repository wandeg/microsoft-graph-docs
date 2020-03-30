---
title: "Get agedAccountsPayable"
description: "Read properties and relationships of the agedAccountsPayable object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get agedAccountsPayable

Namespace: microsoft.graph

Read properties and relationships of the [agedAccountsPayable](../resources/agedaccountspayable.md) object.

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
GET /financials/companies/{companyId}/agedAccountsPayable/{agedAccountsPayableId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [agedAccountsPayable](../resources/agedaccountspayable.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_agedaccountspayable"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/agedAccountsPayable/{agedAccountsPayableId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agedAccountsPayable"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 476

{
  "value": {
    "@odata.type": "#microsoft.graph.agedAccountsPayable",
    "id": "291a900c-900c-291a-0c90-1a290c901a29",
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
}
```

