---
title: "Update taxGroups"
description: "Update the properties of a taxGroups object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update taxGroups

Namespace: microsoft.graph

Update the properties of a taxGroups object.

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
PATCH /financials/companies/{companyId}/taxGroups
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [taxGroup](../resources/taxgroup.md) object.

The following table shows the properties that are required when you create the [taxGroup](../resources/taxgroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|code|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|taxType|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [taxGroup](../resources/taxgroup.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_taxgroups"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/taxGroups
Content-Type: application/json
Content-length: 147

{
  "@odata.type": "#microsoft.graph.taxGroup",
  "code": "Code value",
  "displayName": "Display Name value",
  "taxType": "Tax Type value"
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
  "@odata.type": "#microsoft.graph.taxGroup",
  "id": "25cf1a18-1a18-25cf-181a-cf25181acf25",
  "code": "Code value",
  "displayName": "Display Name value",
  "taxType": "Tax Type value",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00"
}
```

