---
title: "Get importedAppleDeviceIdentity"
description: "Read properties and relationships of the importedAppleDeviceIdentity object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get importedAppleDeviceIdentity

Namespace: microsoft.graph

Read properties and relationships of the [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md) object.

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
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
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
If successful, this method returns a `200 OK` response code and [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_importedappledeviceidentity"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.importedAppleDeviceIdentity"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 668

{
  "value": {
    "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
    "id": "eccf6fd6-6fd6-eccf-d66f-cfecd66fcfec",
    "serialNumber": "Serial Number value",
    "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
    "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:00:28.7525357+03:00",
    "isSupervised": true,
    "discoverySource": "String",
    "isDeleted": true,
    "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
    "lastContactedDateTime": "2017-01-01T00:03:30.5957753+03:00",
    "description": "Description value",
    "enrollmentState": "String",
    "platform": "String"
  }
}
```

