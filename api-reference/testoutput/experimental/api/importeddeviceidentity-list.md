---
title: "List importedDeviceIdentities"
description: "List properties and relationships of the importedDeviceIdentity objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List importedDeviceIdentities

Namespace: microsoft.graph

List properties and relationships of the [importedDeviceIdentity](../resources/importeddeviceidentity.md) objects.

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
GET /deviceManagement/importedDeviceIdentities
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [importedDeviceIdentity](../resources/importeddeviceidentity.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_importeddeviceidentity"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/importedDeviceIdentities
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.importeddeviceidentity)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 579

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentity",
      "id": "381a5bef-5bef-381a-ef5b-1a38ef5b1a38",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "String",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "lastContactedDateTime": "2016-12-31T23:59:02.6652919+03:00",
      "description": "Description value",
      "enrollmentState": "String",
      "platform": "String"
    }
  ]
}
```

