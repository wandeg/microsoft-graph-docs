---
title: "functions"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# functions

Namespace: microsoft.graph



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
GET /applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}/schema/functions
GET /applications/{applicationsId}/synchronization/templates/{synchronizationTemplateId}/schema/functions
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) collection in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_functions"
}
-->
``` http
GET https://graph.microsoft.com/localtest/applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}/schema/functions
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.attributemappingfunctionschema)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 293

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.attributeMappingFunctionSchema",
      "id": "0d1d87b6-87b6-0d1d-b687-1d0db6871d0d",
      "parameters": [
        {
          "@odata.type": "microsoft.graph.attributeMappingParameterSchema"
        }
      ]
    }
  ]
}
```

