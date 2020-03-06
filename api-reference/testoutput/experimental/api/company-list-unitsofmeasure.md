---
title: "List unitsOfMeasure"
description: "Get the unitOfMeasures from the unitsOfMeasure navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List unitsOfMeasure

Namespace: microsoft.graph

Get the unitOfMeasures from the unitsOfMeasure navigation property.

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
GET /financials/companies/{companyId}/unitsOfMeasure
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [unitOfMeasure](../resources/unitofmeasure.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_unitofmeasure"
}
-->
``` http
GET https://graph.microsoft.com/localtest/financials/companies/{companyId}/unitsOfMeasure
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.unitofmeasure)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 359

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.unitOfMeasure",
      "id": "8eecf566-f566-8eec-66f5-ec8e66f5ec8e",
      "code": "Code value",
      "displayName": "Display Name value",
      "internationalStandardCode": "International Standard Code value",
      "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00"
    }
  ]
}
```

