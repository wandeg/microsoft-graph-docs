---
title: "Update dimension"
description: "Update the properties of a dimension object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update dimension

Namespace: microsoft.graph

Update the properties of a [dimension](../resources/dimension.md) object.

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
PATCH /financials/companies/{companyId}/dimensions/{dimensionId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [dimension](../resources/dimension.md) object.

The following table shows the properties that are required when you create the [dimension](../resources/dimension.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|code|String||
|displayName|String||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [dimension](../resources/dimension.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_dimension"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/dimensions/{dimensionId}
Content-type: application/json
Content-length: 116

{
  "@odata.type": "#microsoft.graph.dimension",
  "code": "Code value",
  "displayName": "Display Name value"
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
Content-Length: 229

{
  "@odata.type": "#microsoft.graph.dimension",
  "id": "3936ab0a-ab0a-3936-0aab-36390aab3639",
  "code": "Code value",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:03:05.9649885+00:00"
}
```

