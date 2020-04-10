---
title: "Add customerPaymentJournals"
description: "Add customerPaymentJournals by posting to the customerPaymentJournals collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add customerPaymentJournals

Namespace: microsoft.graph

Add customerPaymentJournals by posting to the customerPaymentJournals collection.

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
POST /financials/companies/{companyId}/customerPaymentJournals/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [customerPaymentJournal](../resources/customerpaymentjournal.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_customerpaymentjournal_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/customerPaymentJournals
Content-type: application/json
Content-length: 257

{
  "@odata.type": "#microsoft.graph.customerPaymentJournal",
  "code": "Code value",
  "displayName": "Display Name value",
  "balancingAccountId": "2418ee3f-ee3f-2418-3fee-18243fee1824",
  "balancingAccountNumber": "Balancing Account Number value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.customerpaymentjournal"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 370

{
  "@odata.type": "#microsoft.graph.customerPaymentJournal",
  "id": "b5ca4cb6-4cb6-b5ca-b64c-cab5b64ccab5",
  "code": "Code value",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
  "balancingAccountId": "2418ee3f-ee3f-2418-3fee-18243fee1824",
  "balancingAccountNumber": "Balancing Account Number value"
}
```

