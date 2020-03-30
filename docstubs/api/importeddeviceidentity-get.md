---
title: "Get importedDeviceIdentity"
description: "Read properties and relationships of the importedDeviceIdentity object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get importedDeviceIdentity

Namespace: microsoft.graph

Read properties and relationships of the [importedDeviceIdentity](../resources/importeddeviceidentity.md) object.

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
GET /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [importedDeviceIdentity](../resources/importeddeviceidentity.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_importeddeviceidentity"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.importedDeviceIdentity"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 546

{
  "value": {
    "@odata.type": "#microsoft.graph.importedDeviceIdentity",
    "id": "13a7c562-c562-13a7-62c5-a71362c5a713",
    "importedDeviceIdentifier": "Imported Device Identifier value",
    "importedDeviceIdentityType": "String",
    "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
    "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
    "lastContactedDateTime": "2016-12-31T23:59:21.9478215+03:00",
    "description": "Description value",
    "enrollmentState": "String",
    "platform": "String"
  }
}
```

