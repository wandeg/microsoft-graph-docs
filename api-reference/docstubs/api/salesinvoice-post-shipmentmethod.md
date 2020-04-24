---
title: "Create shipmentMethod"
description: "Create a new shipmentMethod object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create shipmentMethod

Namespace: microsoft.graph

Create a new shipmentMethod object.

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
POST /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/shipmentMethod
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [shipmentMethod](../resources/shipmentmethod.md) object.

The following table shows the properties that are required when you create the [shipmentMethod](../resources/shipmentmethod.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|code|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [shipmentMethod](../resources/shipmentmethod.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_shipmentmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/shipmentMethod
Content-Type: application/json
Content-length: 121

{
  "@odata.type": "#microsoft.graph.shipmentMethod",
  "code": "Code value",
  "displayName": "Display Name value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shipmentmethod"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.shipmentMethod",
  "id": "a81e4c05-4c05-a81e-054c-1ea8054c1ea8",
  "code": "Code value",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00"
}
```

