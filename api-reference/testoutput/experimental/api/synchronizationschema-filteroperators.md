---
title: "filterOperators"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# filterOperators

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
GET /applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}/schema/filterOperators
GET /applications/{applicationsId}/synchronization/templates/{synchronizationTemplateId}/schema/filterOperators
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [filterOperatorSchema](../resources/filteroperatorschema.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}
-->
``` http
GET https://graph.microsoft.com/localtest/applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}/schema/filterOperators
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.filteroperatorschema)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 288

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.filterOperatorSchema",
      "id": "fd552756-2756-fd55-5627-55fd562755fd",
      "arity": "String",
      "multivaluedComparisonType": "String",
      "supportedAttributeTypes": [
        "String"
      ]
    }
  ]
}
```

