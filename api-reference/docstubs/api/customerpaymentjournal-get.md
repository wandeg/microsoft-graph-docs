---
title: "Get customerPaymentJournal"
description: "Read the properties and relationships of a customerPaymentJournal object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get customerPaymentJournal

Namespace: microsoft.graph

Read the properties and relationships of a [customerPaymentJournal](../resources/customerpaymentjournal.md) object.

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
GET /financials/companies/{companyId}/customerPaymentJournals/{customerPaymentJournalId}
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
If successful, this method returns a `200 OK` response code and a [customerPaymentJournal](../resources/customerpaymentjournal.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_customerpaymentjournal"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/customerPaymentJournals/{customerPaymentJournalId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.customerPaymentJournal"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.customerPaymentJournal",
    "id": "ab303df0-3df0-ab30-f03d-30abf03d30ab",
    "code": "Code value",
    "displayName": "Display Name value",
    "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
    "balancingAccountId": "533bbec1-bec1-533b-c1be-3b53c1be3b53",
    "balancingAccountNumber": "Balancing Account Number value"
  }
}
```

