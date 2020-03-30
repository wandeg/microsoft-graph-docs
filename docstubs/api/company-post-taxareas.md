---
title: "Add taxAreas"
description: "Add taxAreas by posting to the taxAreas collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add taxAreas

Namespace: microsoft.graph

Add taxAreas by posting to the taxAreas collection.

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
POST /financials/companies/{companyId}/taxAreas/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [taxArea](../resources/taxarea.md) object.

The following table shows the properties that are required when you create the [taxArea](../resources/taxarea.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|code|String||
|displayName|String||
|taxType|String||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [taxArea](../resources/taxarea.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_taxarea_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/taxAreas
Content-type: application/json
Content-length: 146

{
  "@odata.type": "#microsoft.graph.taxArea",
  "code": "Code value",
  "displayName": "Display Name value",
  "taxType": "Tax Type value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.taxarea"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 259

{
  "@odata.type": "#microsoft.graph.taxArea",
  "id": "bf8549b3-49b3-bf85-b349-85bfb34985bf",
  "code": "Code value",
  "displayName": "Display Name value",
  "taxType": "Tax Type value",
  "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00"
}
```

