---
title: "Update dimensionValue"
description: "Update the properties of a dimensionValue object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update dimensionValue

Namespace: microsoft.graph

Update the properties of a [dimensionValue](../resources/dimensionvalue.md) object.

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
PATCH /financials/companies/{companyId}/dimensionValues/{dimensionValueId}
PATCH /financials/companies/{companyId}/dimensions/{dimensionId}/dimensionValues/{dimensionValueId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [dimensionValue](../resources/dimensionvalue.md) object.

The following table shows the properties that are required when you create the [dimensionValue](../resources/dimensionvalue.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|code|String||
|displayName|String||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [dimensionValue](../resources/dimensionvalue.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_dimensionvalue"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/dimensionValues/{dimensionValueId}
Content-type: application/json
Content-length: 121

{
  "@odata.type": "#microsoft.graph.dimensionValue",
  "code": "Code value",
  "displayName": "Display Name value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 234

{
  "@odata.type": "#microsoft.graph.dimensionValue",
  "id": "1d808cee-8cee-1d80-ee8c-801dee8c801d",
  "code": "Code value",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00"
}
```

