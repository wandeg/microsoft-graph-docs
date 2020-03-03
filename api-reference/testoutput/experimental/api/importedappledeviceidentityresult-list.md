---
title: "List importedAppleDeviceIdentityResults"
description: "List properties and relationships of the importedAppleDeviceIdentityResult objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List importedAppleDeviceIdentityResults

Namespace: microsoft.graph

List properties and relationships of the [importedAppleDeviceIdentityResult](../resources/importedappledeviceidentityresult.md) objects.

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
GET ** Collection URI for microsoft.graph.importedAppleDeviceIdentityResult not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [importedAppleDeviceIdentityResult](../resources/importedappledeviceidentityresult.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_importedappledeviceidentityresult"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.importedAppleDeviceIdentityResult not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.importedappledeviceidentityresult)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 736

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
      "id": "87ce4481-4481-87ce-8144-ce878144ce87",
      "serialNumber": "Serial Number value",
      "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
      "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:19.9727635+03:00",
      "isSupervised": true,
      "discoverySource": "String",
      "isDeleted": true,
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "lastContactedDateTime": "2016-12-31T23:59:02.6652919+03:00",
      "description": "Description value",
      "enrollmentState": "String",
      "platform": "String",
      "status": true
    }
  ]
}
```

