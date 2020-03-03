---
title: "List directoryObjectPartnerReferences"
description: "List properties and relationships of the directoryObjectPartnerReference objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List directoryObjectPartnerReferences

List properties and relationships of the [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md) objects.

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
GET ** Collection URI for microsoft.graph.directoryObjectPartnerReference not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_directoryobjectpartnerreference"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.directoryObjectPartnerReference not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.directoryobjectpartnerreference)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 429

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.directoryObjectPartnerReference",
      "id": "8ecfcf20-cf20-8ecf-20cf-cf8e20cfcf8e",
      "deletedDateTime": "2017-01-01T00:00:34.0507931+03:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "externalPartnerTenantId": "7b00ec38-ec38-7b00-38ec-007b38ec007b",
      "objectType": "Object Type value"
    }
  ]
}
```

