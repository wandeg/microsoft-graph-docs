---
title: "Update account"
description: "Update the properties of an account object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update account

Namespace: microsoft.graph

Update the properties of an account object.

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
PATCH /financials/companies/{companyId}/journals/{journalId}/journalLines/{journalLineId}/account
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [account](../resources/account.md) object.

The following table shows the properties that are required when you create the [account](../resources/account.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|number|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|category|String|**TODO: Add Description**|
|subCategory|String|**TODO: Add Description**|
|blocked|Boolean|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [account](../resources/account.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_account"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/journals/{journalId}/journalLines/{journalLineId}/account
Content-Type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.account",
  "number": "Number value",
  "displayName": "Display Name value",
  "category": "Category value",
  "subCategory": "Sub Category value",
  "blocked": true
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
  "@odata.type": "#microsoft.graph.account",
  "id": "18b8a962-a962-18b8-62a9-b81862a9b818",
  "number": "Number value",
  "displayName": "Display Name value",
  "category": "Category value",
  "subCategory": "Sub Category value",
  "blocked": true,
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00"
}
```

