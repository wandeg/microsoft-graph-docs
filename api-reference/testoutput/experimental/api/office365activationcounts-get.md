---
title: "Get office365ActivationCounts"
description: "Read properties and relationships of the office365ActivationCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get office365ActivationCounts

Read properties and relationships of the [office365ActivationCounts](../resources/office365activationcounts.md) object.

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
GET ** Entity URI for microsoft.graph.office365ActivationCounts not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [office365ActivationCounts](../resources/office365activationcounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_office365activationcounts"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.office365ActivationCounts not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationCounts"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 311

{
  "value": {
    "@odata.type": "#microsoft.graph.office365ActivationCounts",
    "id": "fb5316b0-16b0-fb53-b016-53fbb01653fb",
    "reportRefreshDate": "Date",
    "productType": "Product Type value",
    "windows": 7,
    "mac": 3,
    "android": 7,
    "ios": 3,
    "windows10Mobile": 15
  }
}
```

