---
title: "Create item"
description: "Create a new item object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create item

Namespace: microsoft.graph

Create a new item object.

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
POST /financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/salesCreditMemoLines/{salesCreditMemoLineId}/item
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [item](../resources/item.md) object.

The following table shows the properties that are required when you create the [item](../resources/item.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|number|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|
|itemCategoryId|Guid|**TODO: Add Description**|
|itemCategoryCode|String|**TODO: Add Description**|
|blocked|Boolean|**TODO: Add Description**|
|baseUnitOfMeasureId|Guid|**TODO: Add Description**|
|gtin|String|**TODO: Add Description**|
|inventory|Decimal|**TODO: Add Description**|
|unitPrice|Decimal|**TODO: Add Description**|
|priceIncludesTax|Boolean|**TODO: Add Description**|
|unitCost|Decimal|**TODO: Add Description**|
|taxGroupId|Guid|**TODO: Add Description**|
|taxGroupCode|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [item](../resources/item.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_item_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/salesCreditMemoLines/{salesCreditMemoLineId}/item
Content-Type: application/json
Content-length: 428

{
  "@odata.type": "#microsoft.graph.item",
  "number": "String",
  "displayName": "String",
  "type": "String",
  "itemCategoryId": "Guid",
  "itemCategoryCode": "String",
  "blocked": "Boolean",
  "baseUnitOfMeasureId": "Guid",
  "gtin": "String",
  "inventory": "Decimal",
  "unitPrice": "Decimal",
  "priceIncludesTax": "Boolean",
  "unitCost": "Decimal",
  "taxGroupId": "Guid",
  "taxGroupCode": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.item"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.item",
  "id": "0559707c-707c-0559-7c70-59057c705905",
  "number": "String",
  "displayName": "String",
  "type": "String",
  "itemCategoryId": "Guid",
  "itemCategoryCode": "String",
  "blocked": "Boolean",
  "baseUnitOfMeasureId": "Guid",
  "gtin": "String",
  "inventory": "Decimal",
  "unitPrice": "Decimal",
  "priceIncludesTax": "Boolean",
  "unitCost": "Decimal",
  "taxGroupId": "Guid",
  "taxGroupCode": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

