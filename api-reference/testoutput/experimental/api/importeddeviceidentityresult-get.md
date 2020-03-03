---
title: "Get importedDeviceIdentityResult"
description: "Read properties and relationships of the importedDeviceIdentityResult object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get importedDeviceIdentityResult

Read properties and relationships of the [importedDeviceIdentityResult](../resources/importeddeviceidentityresult.md) object.

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
GET ** Entity URI for microsoft.graph.importedDeviceIdentityResult not found
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
If successful, this method returns a `200 OK` response code and [importedDeviceIdentityResult](../resources/importeddeviceidentityresult.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_importeddeviceidentityresult"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.importedDeviceIdentityResult not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.importedDeviceIdentityResult"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 573

{
  "value": {
    "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
    "id": "1f624535-4535-1f62-3545-621f3545621f",
    "importedDeviceIdentifier": "Imported Device Identifier value",
    "importedDeviceIdentityType": "String",
    "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
    "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
    "lastContactedDateTime": "2016-12-31T23:57:05.6212876+03:00",
    "description": "Description value",
    "enrollmentState": "String",
    "platform": "String",
    "status": true
  }
}
```

