---
title: "Create item"
description: "Create a new item object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create item

Namespace: microsoft.graph

Create a new [item](../resources/item.md) object.

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
POST /financials/companies/{companyId}/items
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_item_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/financials/companies/{companyId}/items
Content-type: application/json
Content-length: 560

{
  "@odata.type": "#microsoft.graph.item",
  "number": "Number value",
  "displayName": "Display Name value",
  "type": "Type value",
  "itemCategoryId": "f6c1027d-027d-f6c1-7d02-c1f67d02c1f6",
  "itemCategoryCode": "Item Category Code value",
  "blocked": true,
  "baseUnitOfMeasureId": "33eceb10-eb10-33ec-10eb-ec3310ebec33",
  "gtin": "Gtin value",
  "inventory": "4.2",
  "unitPrice": "4.2",
  "priceIncludesTax": true,
  "unitCost": "4.2",
  "taxGroupId": "d4a99fdf-9fdf-d4a9-df9f-a9d4df9fa9d4",
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
  "id": "18a35fd7-5fd7-18a3-d75f-a318d75fa318",
  "number": "Number value",
  "displayName": "Display Name value",
  "type": "Type value",
  "itemCategoryId": "f6c1027d-027d-f6c1-7d02-c1f67d02c1f6",
  "itemCategoryCode": "Item Category Code value",
  "blocked": true,
  "baseUnitOfMeasureId": "33eceb10-eb10-33ec-10eb-ec3310ebec33",
  "gtin": "Gtin value",
  "inventory": "4.2",
  "unitPrice": "4.2",
  "priceIncludesTax": true,
  "unitCost": "4.2",
  "taxGroupId": "d4a99fdf-9fdf-d4a9-df9f-a9d4df9fa9d4",
  "taxGroupCode": "Tax Group Code value",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00"
}
```

