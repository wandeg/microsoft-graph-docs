---
title: "List companies"
description: "List properties and relationships of the company objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List companies

Namespace: microsoft.graph

List properties and relationships of the [company](../resources/company.md) objects.

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
GET /financials/companies
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [company](../resources/company.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_company"
}
-->
``` http
GET https://graph.microsoft.com/localtest/financials/companies
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.company)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.company",
      "id": "deae77e1-77e1-deae-e177-aedee177aede",
      "systemVersion": "System Version value",
      "name": "Name value",
      "displayName": "Display Name value",
      "businessProfileId": "Business Profile Id value"
    }
  ]
}
```

