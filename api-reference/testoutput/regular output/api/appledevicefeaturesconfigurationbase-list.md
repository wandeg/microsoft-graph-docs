---
title: "List appleDeviceFeaturesConfigurationBases"
description: "List properties and relationships of the appleDeviceFeaturesConfigurationBase objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List appleDeviceFeaturesConfigurationBases

List properties and relationships of the [appleDeviceFeaturesConfigurationBase](../resources/appledevicefeaturesconfigurationbase.md) objects.

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
GET ** Collection URI for microsoft.graph.appleDeviceFeaturesConfigurationBase not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [appleDeviceFeaturesConfigurationBase](../resources/appledevicefeaturesconfigurationbase.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_appledevicefeaturesconfigurationbase"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.appleDeviceFeaturesConfigurationBase not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.appledevicefeaturesconfigurationbase)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 407

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.appleDeviceFeaturesConfigurationBase",
      "id": "dadf0ac2-0ac2-dadf-c20a-dfdac20adfda",
      "lastModifiedDateTime": "2016-12-31T23:59:09.8413999+03:00",
      "createdDateTime": "2016-12-31T23:57:22.3554145+03:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```

