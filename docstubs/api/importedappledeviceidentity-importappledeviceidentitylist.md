---
title: "importAppleDeviceIdentityList"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# importAppleDeviceIdentityList

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
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|importedAppleDeviceIdentities|[importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md) collection||
|overwriteImportedDeviceIdentities|Boolean||



## Response
If successful, this action returns a `200 OK` response code and a [importedAppleDeviceIdentityResult](../resources/importedappledeviceidentityresult.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "importedappledeviceidentity_importappledeviceidentitylist"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList

Content-type: application/json
Content-length: 778

{
  "importedAppleDeviceIdentities": [
    {
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
  ],
  "overwriteImportedDeviceIdentities": true
}
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
Content-Length: 737

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
      "id": "43445497-5497-4344-9754-444397544443",
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
      "platform": "String",
      "status": true
    }
  ]
}
```

