---
title: "Update taxGroup"
description: "Update the properties of a taxGroup object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update taxGroup

Namespace: microsoft.graph

Update the properties of a [taxGroup](../resources/taxgroup.md) object.

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
PATCH /financials/companies/{companyId}/taxGroups/{taxGroupId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
If successful, this method returns a `200 OK` response code and an updated [taxGroup](../resources/taxgroup.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_taxgroup"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/taxGroups/{taxGroupId}
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.taxGroup",
  "id": "fee94992-4992-fee9-9249-e9fe9249e9fe",
  "code": "Code value",
  "displayName": "Display Name value",
  "taxType": "Tax Type value",
  "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00"
}
```

