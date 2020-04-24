---
title: "Update items"
description: "Update the properties of an items object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update items

Namespace: microsoft.graph

Update the properties of an items object.

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
PATCH /financials/companies/{companyId}/items
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
If successful, this method returns a `200 OK` response code and an updated [item](../resources/item.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_items"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/items
Content-Type: application/json
Content-length: 560

{
  "@odata.type": "#microsoft.graph.item",
  "number": "Number value",
  "displayName": "Display Name value",
  "type": "Type value",
  "itemCategoryId": "319af97f-f97f-319a-7ff9-9a317ff99a31",
  "itemCategoryCode": "Item Category Code value",
  "blocked": true,
  "baseUnitOfMeasureId": "f477db3a-db3a-f477-3adb-77f43adb77f4",
  "gtin": "Gtin value",
  "inventory": "4.2",
  "unitPrice": "4.2",
  "priceIncludesTax": true,
  "unitCost": "4.2",
  "taxGroupId": "719400e4-00e4-7194-e400-9471e4009471",
  "taxGroupCode": "Tax Group Code value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.item",
  "id": "8839c4c9-c4c9-8839-c9c4-3988c9c43988",
  "number": "Number value",
  "displayName": "Display Name value",
  "type": "Type value",
  "itemCategoryId": "319af97f-f97f-319a-7ff9-9a317ff99a31",
  "itemCategoryCode": "Item Category Code value",
  "blocked": true,
  "baseUnitOfMeasureId": "f477db3a-db3a-f477-3adb-77f43adb77f4",
  "gtin": "Gtin value",
  "inventory": "4.2",
  "unitPrice": "4.2",
  "priceIncludesTax": true,
  "unitCost": "4.2",
  "taxGroupId": "719400e4-00e4-7194-e400-9471e4009471",
  "taxGroupCode": "Tax Group Code value",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00"
}
```

