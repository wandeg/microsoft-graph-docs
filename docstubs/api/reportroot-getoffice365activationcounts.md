---
title: "getOffice365ActivationCounts"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getOffice365ActivationCounts

Namespace: microsoft.graph



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
GET /reports/getOffice365ActivationCounts
GET /print/reports/{reportRootId}/getOffice365ActivationCounts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [office365ActivationCounts](../resources/office365activationcounts.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.office365activationcounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 343

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.office365ActivationCounts",
      "id": "e46de195-e195-e46d-95e1-6de495e16de4",
      "reportRefreshDate": "Date",
      "productType": "Product Type value",
      "windows": 7,
      "mac": 3,
      "android": 7,
      "ios": 3,
      "windows10Mobile": 15
    }
  ]
}
```

