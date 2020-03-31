---
title: "Update customerPaymentJournal"
description: "Update the properties of a customerPaymentJournal object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update customerPaymentJournal

Namespace: microsoft.graph

Update the properties of a [customerPaymentJournal](../resources/customerpaymentjournal.md) object.

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
PATCH /financials/companies/{companyId}/customerPaymentJournals/{customerPaymentJournalId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [customerPaymentJournal](../resources/customerpaymentjournal.md) object.

The following table shows the properties that are required when you create the [customerPaymentJournal](../resources/customerpaymentjournal.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|code|String||
|displayName|String||
|lastModifiedDateTime|DateTimeOffset||
|balancingAccountId|Guid||
|balancingAccountNumber|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [customerPaymentJournal](../resources/customerpaymentjournal.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_customerpaymentjournal"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/customerPaymentJournals/{customerPaymentJournalId}
Content-type: application/json
Content-length: 257

{
  "@odata.type": "#microsoft.graph.customerPaymentJournal",
  "code": "Code value",
  "displayName": "Display Name value",
  "balancingAccountId": "33875c5d-5c5d-3387-5d5c-87335d5c8733",
  "balancingAccountNumber": "Balancing Account Number value"
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
Content-Length: 370

{
  "@odata.type": "#microsoft.graph.customerPaymentJournal",
  "id": "e4584ac5-4ac5-e458-c54a-58e4c54a58e4",
  "code": "Code value",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00",
  "balancingAccountId": "33875c5d-5c5d-3387-5d5c-87335d5c8733",
  "balancingAccountNumber": "Balancing Account Number value"
}
```

