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

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /financials/companies/{companyId}/customerPaymentJournals
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [customerPaymentJournal](../resources/customerpaymentjournal.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_customerpaymentjournal"
}
-->
``` http
GET https://graph.microsoft.com/localtest/financials/companies/{companyId}/customerPaymentJournals
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
      "id": "eb324685-4685-eb32-8546-32eb854632eb",
      "code": "Code value",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
      "balancingAccountId": "4d5af2d7-f2d7-4d5a-d7f2-5a4dd7f25a4d",
      "balancingAccountNumber": "Balancing Account Number value"
    }
  ]
}
```

