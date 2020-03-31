---
title: "Add taxGroups"
description: "Add taxGroups by posting to the taxGroups collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add taxGroups

Namespace: microsoft.graph

Add taxGroups by posting to the taxGroups collection.

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
POST /financials/companies/{companyId}/taxGroups/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [taxGroup](../resources/taxgroup.md) object.

The following table shows the properties that are required when you create the [taxGroup](../resources/taxgroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|code|String||
|displayName|String||
|taxType|String||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [taxGroup](../resources/taxgroup.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_taxgroup_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/taxGroups
Content-type: application/json
Content-length: 147

{
  "@odata.type": "#microsoft.graph.taxGroup",
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
  "@odata.type": "microsoft.graph.taxgroup"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.taxGroup",
  "id": "aff0d679-d679-aff0-79d6-f0af79d6f0af",
  "code": "Code value",
  "displayName": "Display Name value",
  "taxType": "Tax Type value",
  "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00"
}
```

