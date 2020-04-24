---
title: "List managedDevices"
description: "Get the managedDevices from the managedDevices navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List managedDevices

Namespace: microsoft.graph

Get the managedDevices from the managedDevices navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /invitations/{invitationsId}/invitedUser/managedDevices/{managedDeviceId}/detectedApps/{detectedAppId}/managedDevices
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [managedDevice](../resources/manageddevice.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_manageddevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/managedDevices/{managedDeviceId}/detectedApps/{detectedAppId}/managedDevices
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.manageddevice)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDevice",
      "id": "49a11602-1602-49a1-0216-a1490216a149",
      "userId": "User Id value",
      "deviceName": "Device Name value",
      "hardwareInformation": {
        "@odata.type": "microsoft.graph.hardwareInformation",
        "serialNumber": "Serial Number value",
        "totalStorageSpace": 1,
        "freeStorageSpace": 0,
        "imei": "Imei value",
        "meid": "Meid value",
        "manufacturer": "Manufacturer value",
        "model": "Model value",
        "phoneNumber": "Phone Number value",
        "subscriberCarrier": "Subscriber Carrier value",
        "cellularTechnology": "Cellular Technology value",
        "wifiMac": "Wifi Mac value",
        "operatingSystemLanguage": "Operating System Language value",
        "isSupervised": true,
        "isEncrypted": true,
        "isSharedDevice": true,
        "sharedDeviceCachedUsers": [
          {
            "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
            "userPrincipalName": "User Principal Name value",
            "dataToSync": true,
            "dataQuota": 9,
            "dataUsed": 8
          }
        ],
        "tpmSpecificationVersion": "Tpm Specification Version value",
        "operatingSystemEdition": "Operating System Edition value",
        "deviceFullQualifiedDomainName": "Device Full Qualified Domain Name value",
        "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
        "deviceGuardVirtualizationBasedSecurityState": "String",
        "deviceGuardLocalSystemAuthorityCredentialGuardState": "String",
        "osBuildNumber": "Os Build Number value"
      },
      "ownerType": "String",
      "managedDeviceOwnerType": "String",
      "deviceActionResults": [
        {
          "@odata.type": "microsoft.graph.deviceActionResult",
          "actionName": "Action Name value",
          "actionState": "String",
          "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
          "lastUpdatedDateTime": "2016-12-31T23:58:57.2159356+03:00"
        }
      ],
      "managementState": "String",
      "enrolledDateTime": "2016-12-31T23:58:55.5615826+03:00",
      "lastSyncDateTime": "2017-01-01T00:02:17.5414184+03:00",
      "chassisType": "String",
      "operatingSystem": "Operating System value",
      "deviceType": "String",
      "complianceState": "String",
      "jailBroken": "Jail Broken value",
      "managementAgent": "String",
      "osVersion": "Os Version value",
      "easActivated": true,
      "easDeviceId": "Eas Device Id value",
      "easActivationDateTime": "2017-01-01T00:02:07.1458063+03:00",
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
      "exchangeLastSuccessfulSyncDateTime": "2016-12-31T23:58:22.4386883+03:00",
      "exchangeAccessState": "String",
      "exchangeAccessStateReason": "String",
      "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
      "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
      "isEncrypted": true,
      "userPrincipalName": "User Principal Name value",
      "model": "Model value",
      "manufacturer": "Manufacturer value",
      "imei": "Imei value",
      "complianceGracePeriodExpirationDateTime": "2017-01-01T00:02:41.4369203+03:00",
      "serialNumber": "Serial Number value",
      "phoneNumber": "Phone Number value",
      "androidSecurityPatchLevel": "Android Security Patch Level value",
      "userDisplayName": "User Display Name value",
      "configurationManagerClientEnabledFeatures": {
        "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
        "inventory": true,
        "modernApps": true,
        "resourceAccess": true,
        "deviceConfiguration": true,
        "compliancePolicy": true,
        "windowsUpdateForBusiness": true,
        "endpointProtection": true,
        "officeApps": true
      },
      "wiFiMacAddress": "Wi Fi Mac Address value",
      "deviceHealthAttestationState": {
        "@odata.type": "microsoft.graph.deviceHealthAttestationState",
        "lastUpdateDateTime": "Last Update Date Time value",
        "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
        "deviceHealthAttestationStatus": "Device Health Attestation Status value",
        "contentVersion": "Content Version value",
        "issuedDateTime": "2017-01-01T00:03:23.0546586+03:00",
        "attestationIdentityKey": "Attestation Identity Key value",
        "resetCount": 10,
        "restartCount": 12,
        "dataExcutionPolicy": "Data Excution Policy value",
        "bitLockerStatus": "Bit Locker Status value",
        "bootManagerVersion": "Boot Manager Version value",
        "codeIntegrityCheckVersion": "Code Integrity Check Version value",
        "secureBoot": "Secure Boot value",
        "bootDebugging": "Boot Debugging value",
        "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
        "codeIntegrity": "Code Integrity value",
        "testSigning": "Test Signing value",
        "safeMode": "Safe Mode value",
        "windowsPE": "Windows PE value",
        "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
        "virtualSecureMode": "Virtual Secure Mode value",
        "pcrHashAlgorithm": "Pcr Hash Algorithm value",
        "bootAppSecurityVersion": "Boot App Security Version value",
        "bootManagerSecurityVersion": "Boot Manager Security Version value",
        "tpmVersion": "Tpm Version value",
        "pcr0": "Pcr0 value",
        "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
        "codeIntegrityPolicy": "Code Integrity Policy value",
        "bootRevisionListInfo": "Boot Revision List Info value",
        "operatingSystemRevListInfo": "Operating System Rev List Info value",
        "healthStatusMismatchInfo": "Health Status Mismatch Info value",
        "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
      },
      "subscriberCarrier": "Subscriber Carrier value",
      "meid": "Meid value",
      "totalStorageSpaceInBytes": 8,
      "freeStorageSpaceInBytes": 7,
      "managedDeviceName": "Managed Device Name value",
      "partnerReportedThreatState": "String",
      "retireAfterDateTime": "2017-01-01T00:02:41.3283665+03:00",
      "usersLoggedOn": [
        {
          "@odata.type": "microsoft.graph.loggedOnUser",
          "lastLogOnDateTime": "2016-12-31T23:56:35.4732637+03:00"
        }
      ],
      "preferMdmOverGroupPolicyAppliedDateTime": "2017-01-01T00:00:17.4101662+03:00",
      "autopilotEnrolled": true,
      "requireUserEnrollmentApproval": true,
      "managementCertificateExpirationDate": "2016-12-31T23:58:43.1896279+03:00",
      "iccid": "Iccid value",
      "udid": "Udid value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "windowsActiveMalwareCount": 9,
      "windowsRemediatedMalwareCount": 13,
      "notes": "Notes value",
      "configurationManagerClientHealthState": {
        "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
        "state": "String",
        "errorCode": 9
      },
      "configurationManagerClientInformation": {
        "@odata.type": "microsoft.graph.configurationManagerClientInformation",
        "clientIdentifier": "Client Identifier value",
        "isBlocked": true
      },
      "ethernetMacAddress": "Ethernet Mac Address value",
      "physicalMemoryInBytes": 5,
      "processorArchitecture": "String",
      "specificationVersion": "Specification Version value"
    }
  ]
}
```

