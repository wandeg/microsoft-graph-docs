---
title: "List customerPaymentJournals"
description: "Get the customerPaymentJournals from the customerPaymentJournals navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List customerPaymentJournals

Namespace: microsoft.graph

Get the customerPaymentJournals from the customerPaymentJournals navigation property.

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
GET /financials/companies/{companyId}/customerPaymentJournals
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
If successful, this method returns a `200 OK` response code and a collection of [customerPaymentJournal](../resources/customerpaymentjournal.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_customerpaymentjournal"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/customerPaymentJournals
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.customerpaymentjournal)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 431

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.customerPaymentJournal",
      "id": "178c0098-0098-178c-9800-8c1798008c17",
      "code": "Code value",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
      "balancingAccountId": "bf72f268-f268-bf72-68f2-72bf68f272bf",
      "balancingAccountNumber": "Balancing Account Number value"
    }
  ]
}
```

