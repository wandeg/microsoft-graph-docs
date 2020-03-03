---
title: "List accounts"
description: "Get the accounts from the accounts navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List accounts

Get the accounts from the accounts navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /financials/companies/{companyId}/accounts
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [account](../resources/account.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_account"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/financials/companies/{companyId}/accounts
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.account)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 389

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.account",
      "id": "d1679b19-9b19-d167-199b-67d1199b67d1",
      "number": "Number value",
      "displayName": "Display Name value",
      "category": "Category value",
      "subCategory": "Sub Category value",
      "blocked": true,
      "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00"
    }
  ]
}
```

