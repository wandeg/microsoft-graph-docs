---
title: "List androidImportedPFXCertificateProfiles"
description: "List properties and relationships of the androidImportedPFXCertificateProfile objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List androidImportedPFXCertificateProfiles

Namespace: microsoft.graph

List properties and relationships of the [androidImportedPFXCertificateProfile](../resources/androidimportedpfxcertificateprofile.md) objects.

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
GET ** Collection URI for microsoft.graph.androidImportedPFXCertificateProfile not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [androidImportedPFXCertificateProfile](../resources/androidimportedpfxcertificateprofile.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_androidimportedpfxcertificateprofile"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.androidImportedPFXCertificateProfile not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.androidimportedpfxcertificateprofile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1657

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
      "id": "25b90af9-0af9-25b9-f90a-b925f90ab925",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "deviceManagementApplicabilityRuleOsEdition": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
        "osEditionTypes": [
          "String"
        ],
        "name": "Name value",
        "ruleType": "String"
      },
      "deviceManagementApplicabilityRuleOsVersion": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
        "minOSVersion": "Min OSVersion value",
        "maxOSVersion": "Max OSVersion value"
      },
      "deviceManagementApplicabilityRuleDeviceMode": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
        "deviceMode": "String"
      },
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "renewalThresholdPercentage": 10,
      "subjectNameFormat": "String",
      "subjectAlternativeNameType": "String",
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "String",
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "objectIdentifier": "Object Identifier value"
        }
      ],
      "intendedPurpose": "String"
    }
  ]
}
```

