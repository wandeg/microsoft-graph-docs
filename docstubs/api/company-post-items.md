---
title: "Add items"
description: "Add items by posting to the items collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add items

Namespace: microsoft.graph

Add items by posting to the items collection.

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
POST /financials/companies/{companyId}/items/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [item](../resources/item.md) object.

The following table shows the properties that are required when you create the [item](../resources/item.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|number|String||
|displayName|String||
|type|String||
|itemCategoryId|Guid||
|itemCategoryCode|String||
|blocked|Boolean||
|baseUnitOfMeasureId|Guid||
|gtin|String||
|inventory|Decimal||
|unitPrice|Decimal||
|priceIncludesTax|Boolean||
|unitCost|Decimal||
|taxGroupId|Guid||
|taxGroupCode|String||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [item](../resources/item.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_item_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/items
Content-type: application/json
Content-length: 560

{
  "@odata.type": "#microsoft.graph.item",
  "number": "Number value",
  "displayName": "Display Name value",
  "type": "Type value",
  "itemCategoryId": "06d0fe0d-fe0d-06d0-0dfe-d0060dfed006",
  "itemCategoryCode": "Item Category Code value",
  "blocked": true,
  "baseUnitOfMeasureId": "3f0cfef8-fef8-3f0c-f8fe-0c3ff8fe0c3f",
  "gtin": "Gtin value",
  "inventory": "4.2",
  "unitPrice": "4.2",
  "priceIncludesTax": true,
  "unitCost": "4.2",
  "taxGroupId": "0641b09e-b09e-0641-9eb0-41069eb04106",
  "taxGroupCode": "Tax Group Code value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.item"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 673

{
  "@odata.type": "#microsoft.graph.item",
  "id": "1c186fde-6fde-1c18-de6f-181cde6f181c",
  "number": "Number value",
  "displayName": "Display Name value",
  "type": "Type value",
  "itemCategoryId": "06d0fe0d-fe0d-06d0-0dfe-d0060dfed006",
  "itemCategoryCode": "Item Category Code value",
  "blocked": true,
  "baseUnitOfMeasureId": "3f0cfef8-fef8-3f0c-f8fe-0c3ff8fe0c3f",
  "gtin": "Gtin value",
  "inventory": "4.2",
  "unitPrice": "4.2",
  "priceIncludesTax": true,
  "unitCost": "4.2",
  "taxGroupId": "0641b09e-b09e-0641-9eb0-41069eb04106",
  "taxGroupCode": "Tax Group Code value",
  "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00"
}
```

