---
title: "Get appleDeviceFeaturesConfigurationBase"
description: "Read properties and relationships of the appleDeviceFeaturesConfigurationBase object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get appleDeviceFeaturesConfigurationBase

Read properties and relationships of the [appleDeviceFeaturesConfigurationBase](../resources/appledevicefeaturesconfigurationbase.md) object.

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
GET ** Entity URI for microsoft.graph.appleDeviceFeaturesConfigurationBase not found
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
If successful, this method returns a `200 OK` response code and [appleDeviceFeaturesConfigurationBase](../resources/appledevicefeaturesconfigurationbase.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_appledevicefeaturesconfigurationbase"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.appleDeviceFeaturesConfigurationBase not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appleDeviceFeaturesConfigurationBase"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 379

{
  "value": {
    "@odata.type": "#microsoft.graph.appleDeviceFeaturesConfigurationBase",
    "id": "dadf0ac2-0ac2-dadf-c20a-dfdac20adfda",
    "lastModifiedDateTime": "2016-12-31T23:59:09.8413999+03:00",
    "createdDateTime": "2016-12-31T23:57:22.3554145+03:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```

