---
title: "List items"
description: "Get the items from the items navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List items

Namespace: microsoft.graph

Get the items from the items navigation property.

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
GET /financials/companies/{companyId}/items
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
If successful, this method returns a `200 OK` response code and a collection of [item](../resources/item.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_item"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/items
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.item)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 774

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.item",
      "id": "d9f47e77-7e77-d9f4-777e-f4d9777ef4d9",
      "number": "Number value",
      "displayName": "Display Name value",
      "type": "Type value",
      "itemCategoryId": "2f905af9-5af9-2f90-f95a-902ff95a902f",
      "itemCategoryCode": "Item Category Code value",
      "blocked": true,
      "baseUnitOfMeasureId": "c4a55195-5195-c4a5-9551-a5c49551a5c4",
      "gtin": "Gtin value",
      "inventory": "4.2",
      "unitPrice": "4.2",
      "priceIncludesTax": true,
      "unitCost": "4.2",
      "taxGroupId": "1be4f5fb-f5fb-1be4-fbf5-e41bfbf5e41b",
      "taxGroupCode": "Tax Group Code value",
      "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00"
    }
  ]
}
```

