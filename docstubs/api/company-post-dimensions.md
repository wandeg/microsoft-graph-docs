---
title: "Add dimensions"
description: "Add dimensions by posting to the dimensions collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add dimensions

Namespace: microsoft.graph

Add dimensions by posting to the dimensions collection.

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
POST /financials/companies/{companyId}/dimensions/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [dimension](../resources/dimension.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_dimension_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/dimensions
Content-type: application/json
Content-length: 116

{
  "@odata.type": "#microsoft.graph.dimension",
  "code": "Code value",
  "displayName": "Display Name value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.dimension"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 229

{
  "@odata.type": "#microsoft.graph.dimension",
  "id": "5ca278ce-78ce-5ca2-ce78-a25cce78a25c",
  "code": "Code value",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00"
}
```

