---
title: "Add dimensionValues"
description: "Add dimensionValues by posting to the dimensionValues collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add dimensionValues

Namespace: microsoft.graph

Add dimensionValues by posting to the dimensionValues collection.

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
POST /financials/companies/{companyId}/dimensionValues/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [dimensionValue](../resources/dimensionvalue.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_dimensionvalue_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/dimensionValues
Content-type: application/json
Content-length: 121

{
  "@odata.type": "#microsoft.graph.dimensionValue",
  "code": "Code value",
  "displayName": "Display Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.dimensionvalue"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 234

{
  "@odata.type": "#microsoft.graph.dimensionValue",
  "id": "466b77f3-77f3-466b-f377-6b46f3776b46",
  "code": "Code value",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00"
}
```

