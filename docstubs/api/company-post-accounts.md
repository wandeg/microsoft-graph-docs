---
title: "Add accounts"
description: "Add accounts by posting to the accounts collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add accounts

Namespace: microsoft.graph

Add accounts by posting to the accounts collection.

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
POST /financials/companies/{companyId}/accounts/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [account](../resources/account.md) object.

The following table shows the properties that are required when you create the [account](../resources/account.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|number|String||
|displayName|String||
|category|String||
|subCategory|String||
|blocked|Boolean||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [account](../resources/account.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_account_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/accounts
Content-type: application/json
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.account"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 323

{
  "@odata.type": "#microsoft.graph.account",
  "id": "a3c7e806-e806-a3c7-06e8-c7a306e8c7a3",
  "number": "Number value",
  "displayName": "Display Name value",
  "category": "Category value",
  "subCategory": "Sub Category value",
  "blocked": true,
  "lastModifiedDateTime": "2017-01-01T00:02:23.471109+03:00"
}
```

