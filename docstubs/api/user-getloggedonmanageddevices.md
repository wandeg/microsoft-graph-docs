---
title: "getLoggedOnManagedDevices"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getLoggedOnManagedDevices

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
GET /me/getLoggedOnManagedDevices
GET /users/{usersId}/getLoggedOnManagedDevices
GET /me/managedDevices/{managedDeviceId}/users/{userId}/getLoggedOnManagedDevices
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [managedDevice](../resources/manageddevice.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "user_getloggedonmanageddevices"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/getLoggedOnManagedDevices
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.manageddevice)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4166

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDevice",
      "id": "39cc1c6e-1c6e-39cc-6e1c-cc396e1ccc39",
      "userId": "User Id value",
      "deviceName": "Device Name value",
      "hardwareInformation": {
        "@odata.type": "microsoft.graph.hardwareInformation"
      },
      "ownerType": "String",
      "managedDeviceOwnerType": "String",
      "deviceActionResults": [
        {
          "@odata.type": "microsoft.graph.deviceActionResult"
        }
      ],
      "managementState": "String",
      "enrolledDateTime": "2017-01-01T00:02:00.9885527+00:00",
      "lastSyncDateTime": "2016-12-31T23:57:21.5163223+00:00",
      "chassisType": "String",
      "operatingSystem": "Operating System value",
      "deviceType": "String",
      "complianceState": "String",
      "jailBroken": "Jail Broken value",
      "managementAgent": "String",
      "osVersion": "Os Version value",
      "easActivated": true,
      "easDeviceId": "Eas Device Id value",
      "easActivationDateTime": "2016-12-31T23:58:48.6993193+00:00",
      "aadRegistered": true,
      "azureADRegistered": true,
      "deviceEnrollmentType": "String",
      "lostModeState": "String",
      "activationLockBypassCode": "Activation Lock Bypass Code value",
      "emailAddress": "Email Address value",
      "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
      "azureADDeviceId": "Azure ADDevice Id value",
      "deviceRegistrationState": "String",
      "deviceCategoryDisplayName": "Device Category Display Name value",
      "isSupervised": true,
      "exchangeLastSuccessfulSyncDateTime": "2016-12-31T23:58:05.7930245+00:00",
      "exchangeAccessState": "String",
      "exchangeAccessStateReason": "String",
      "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
      "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
      "isEncrypted": true,
      "userPrincipalName": "User Principal Name value",
      "model": "Model value",
      "manufacturer": "Manufacturer value",
      "imei": "Imei value",
      "complianceGracePeriodExpirationDateTime": "2017-01-01T00:00:12.5599549+00:00",
      "serialNumber": "Serial Number value",
      "phoneNumber": "Phone Number value",
      "androidSecurityPatchLevel": "Android Security Patch Level value",
      "userDisplayName": "User Display Name value",
      "configurationManagerClientEnabledFeatures": {
        "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
      },
      "wiFiMacAddress": "Wi Fi Mac Address value",
      "deviceHealthAttestationState": {
        "@odata.type": "microsoft.graph.deviceHealthAttestationState"
      },
      "subscriberCarrier": "Subscriber Carrier value",
      "meid": "Meid value",
      "totalStorageSpaceInBytes": 8,
      "freeStorageSpaceInBytes": 7,
      "managedDeviceName": "Managed Device Name value",
      "partnerReportedThreatState": "String",
      "retireAfterDateTime": "2017-01-01T00:02:27.5718859+00:00",
      "usersLoggedOn": [
        {
          "@odata.type": "microsoft.graph.loggedOnUser"
        }
      ],
      "preferMdmOverGroupPolicyAppliedDateTime": "2017-01-01T00:00:36.7833747+00:00",
      "autopilotEnrolled": true,
      "requireUserEnrollmentApproval": true,
      "managementCertificateExpirationDate": "2016-12-31T23:58:54.2798571+00:00",
      "iccid": "Iccid value",
      "udid": "Udid value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "windowsActiveMalwareCount": 9,
      "windowsRemediatedMalwareCount": 13,
      "notes": "Notes value",
      "configurationManagerClientHealthState": {
        "@odata.type": "microsoft.graph.configurationManagerClientHealthState"
      },
      "configurationManagerClientInformation": {
        "@odata.type": "microsoft.graph.configurationManagerClientInformation"
      },
      "ethernetMacAddress": "Ethernet Mac Address value",
      "physicalMemoryInBytes": 5,
      "processorArchitecture": "String"
    }
  ]
}
```

