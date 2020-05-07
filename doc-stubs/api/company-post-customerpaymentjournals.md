---
title: "Create customerPaymentJournals"
description: "Create a new customerPaymentJournals object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create customerPaymentJournals

Namespace: microsoft.graph

Create a new customerPaymentJournals object.

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
POST /financials/companies/{companyId}/customerPaymentJournals
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [customerPaymentJournal](../resources/customerpaymentjournal.md) object.

The following table shows the properties that are required when you create the [customerPaymentJournal](../resources/customerpaymentjournal.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|code|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|balancingAccountId|Guid|**TODO: Add Description**|
|balancingAccountNumber|String|**TODO: Add Description**|



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
Content-Type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.customerPaymentJournal",
  "code": "String",
  "displayName": "String",
  "balancingAccountId": "Guid",
  "balancingAccountNumber": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.customerpaymentjournal"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.customerPaymentJournal",
  "id": "e6858980-8980-e685-8089-85e6808985e6",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "balancingAccountId": "Guid",
  "balancingAccountNumber": "String"
}
```

