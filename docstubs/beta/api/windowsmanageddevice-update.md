---
title: "Update windowsManagedDevice"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Update windowsManagedDevice

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a windowsManagedDevice object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from most to least privileged) |
| :------------------------------------- | :------------------------------------------ |
| Delegated (work or school account)     |                                             |
| Delegated (personal Microsoft account) |                                             |
| Application                            |                                             |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

```http

```

## Request headers

| Name          | Description                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}. Required.   |
| Content-Type  | application/json. Required. |

## Request body

In the request body, supply JSON representation of the windowsManagedDevice object.

The following table shows the properties that are required when you create the windowsManagedDevice object.

| Property                | Type                           | Description                           |
| :---------------------- | :----------------------------- | :------------------------------------ |
| $(this.Properties.Name) | $(this.Properties.DisplayType) | $(this.Properties.DisplayDescription) |

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [windowsManagedDevice](../resources/windowsManagedDevice.md) object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "update_windowsmanageddevice"
}
-->

```http
PATCH https://graph.microsoft.com/beta/

Content-Type: application/json
Content-Length: 6270

{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
  "aadRegistered": "Boolean",
  "activationLockBypassCode": "String",
  "androidSecurityPatchLevel": "String",
  "autopilotEnrolled": "Boolean",
  "azureADDeviceId": "String",
  "azureADRegistered": "Boolean",
  "azureActiveDirectoryDeviceId": "String",
  "chassisType": "String",
  "complianceGracePeriodExpirationDateTime": "DateTimeOffset",
  "complianceState": "String",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
    "compliancePolicy": "Boolean",
    "deviceConfiguration": "Boolean",
    "endpointProtection": "Boolean",
    "inventory": "Boolean",
    "modernApps": "Boolean",
    "officeApps": "Boolean",
    "resourceAccess": "Boolean",
    "windowsUpdateForBusiness": "Boolean"
  },
  "configurationManagerClientHealthState": {
    "@odata.type": "#microsoft.graph.configurationManagerClientHealthState",
    "errorCode": "Int32",
    "lastSyncDateTime": "DateTimeOffset",
    "state": "String"
  },
  "configurationManagerClientInformation": {
    "@odata.type": "#microsoft.graph.configurationManagerClientInformation",
    "clientIdentifier": "String",
    "isBlocked": "Boolean"
  },
  "deviceActionResults": [
    {
      "@odata.type": "#microsoft.graph.deviceActionResult",
      "actionName": "String",
      "actionState": "String",
      "lastUpdatedDateTime": "DateTimeOffset",
      "startDateTime": "DateTimeOffset"
    }
  ],
  "deviceCategoryDisplayName": "String",
  "deviceEnrollmentType": "String",
  "deviceHealthAttestationState": {
    "@odata.type": "#microsoft.graph.deviceHealthAttestationState",
    "attestationIdentityKey": "String",
    "bitLockerStatus": "String",
    "bootAppSecurityVersion": "String",
    "bootDebugging": "String",
    "bootManagerSecurityVersion": "String",
    "bootManagerVersion": "String",
    "bootRevisionListInfo": "String",
    "codeIntegrity": "String",
    "codeIntegrityCheckVersion": "String",
    "codeIntegrityPolicy": "String",
    "contentNamespaceUrl": "String",
    "contentVersion": "String",
    "dataExcutionPolicy": "String",
    "deviceHealthAttestationStatus": "String",
    "earlyLaunchAntiMalwareDriverProtection": "String",
    "healthAttestationSupportedStatus": "String",
    "healthStatusMismatchInfo": "String",
    "issuedDateTime": "DateTimeOffset",
    "lastUpdateDateTime": "String",
    "operatingSystemKernelDebugging": "String",
    "operatingSystemRevListInfo": "String",
    "pcr0": "String",
    "pcrHashAlgorithm": "String",
    "resetCount": "Int64",
    "restartCount": "Int64",
    "safeMode": "String",
    "secureBoot": "String",
    "secureBootConfigurationPolicyFingerPrint": "String",
    "testSigning": "String",
    "tpmVersion": "String",
    "virtualSecureMode": "String",
    "windowsPE": "String"
  },
  "deviceName": "String",
  "deviceRegistrationState": "String",
  "deviceType": "String",
  "easActivated": "Boolean",
  "easActivationDateTime": "DateTimeOffset",
  "easDeviceId": "String",
  "emailAddress": "String",
  "enrolledDateTime": "DateTimeOffset",
  "ethernetMacAddress": "String",
  "exchangeAccessState": "String",
  "exchangeAccessStateReason": "String",
  "exchangeLastSuccessfulSyncDateTime": "DateTimeOffset",
  "freeStorageSpaceInBytes": "Int64",
  "hardwareInformation": {
    "@odata.type": "#microsoft.graph.hardwareInformation",
    "cellularTechnology": "String",
    "deviceFullQualifiedDomainName": "String",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "String",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
    "deviceGuardVirtualizationBasedSecurityState": "String",
    "freeStorageSpace": "Int64",
    "imei": "String",
    "isEncrypted": "Boolean",
    "isSharedDevice": "Boolean",
    "isSupervised": "Boolean",
    "manufacturer": "String",
    "meid": "String",
    "model": "String",
    "operatingSystemEdition": "String",
    "operatingSystemLanguage": "String",
    "operatingSystemProductType": "Int32",
    "osBuildNumber": "String",
    "phoneNumber": "String",
    "serialNumber": "String",
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "#microsoft.graph.sharedAppleDeviceUser",
        "dataQuota": "Int64",
        "dataToSync": "Boolean",
        "dataUsed": "Int64",
        "userPrincipalName": "String"
      }
    ],
    "subscriberCarrier": "String",
    "totalStorageSpace": "Int64",
    "tpmSpecificationVersion": "String",
    "wifiMac": "String"
  },
  "iccid": "String",
  "imei": "String",
  "isEncrypted": "Boolean",
  "isSupervised": "Boolean",
  "jailBroken": "String",
  "joinType": "String",
  "lastSyncDateTime": "DateTimeOffset",
  "lostModeState": "String",
  "managedDeviceName": "String",
  "managedDeviceOwnerType": "String",
  "managementAgent": "String",
  "managementCertificateExpirationDate": "DateTimeOffset",
  "managementState": "String",
  "manufacturer": "String",
  "meid": "String",
  "model": "String",
  "notes": "String",
  "operatingSystem": "String",
  "osVersion": "String",
  "ownerType": "String",
  "partnerReportedThreatState": "String",
  "phoneNumber": "String",
  "physicalMemoryInBytes": "Int64",
  "preferMdmOverGroupPolicyAppliedDateTime": "DateTimeOffset",
  "processorArchitecture": "String",
  "remoteAssistanceSessionErrorDetails": "String",
  "remoteAssistanceSessionUrl": "String",
  "requireUserEnrollmentApproval": "Boolean",
  "retireAfterDateTime": "DateTimeOffset",
  "roleScopeTagIds": [
    "String"
  ],
  "serialNumber": "String",
  "skuFamily": "String",
  "specificationVersion": "String",
  "subscriberCarrier": "String",
  "totalStorageSpaceInBytes": "Int64",
  "udid": "String",
  "userDisplayName": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "usersLoggedOn": [
    {
      "@odata.type": "#microsoft.graph.loggedOnUser",
      "lastLogOnDateTime": "DateTimeOffset",
      "userId": "String"
    }
  ],
  "wiFiMacAddress": "String",
  "windowsActiveMalwareCount": "Int32",
  "windowsRemediatedMalwareCount": "Int32"
}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.windowsManagedDevice"
}
-->

```http
HTTP 1.1 200 OK

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
  "aadRegistered": "Boolean",
  "activationLockBypassCode": "String",
  "androidSecurityPatchLevel": "String",
  "autopilotEnrolled": "Boolean",
  "azureADDeviceId": "String",
  "azureADRegistered": "Boolean",
  "azureActiveDirectoryDeviceId": "String",
  "chassisType": "String",
  "complianceGracePeriodExpirationDateTime": "DateTimeOffset",
  "complianceState": "String",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
    "compliancePolicy": "Boolean",
    "deviceConfiguration": "Boolean",
    "endpointProtection": "Boolean",
    "inventory": "Boolean",
    "modernApps": "Boolean",
    "officeApps": "Boolean",
    "resourceAccess": "Boolean",
    "windowsUpdateForBusiness": "Boolean"
  },
  "configurationManagerClientHealthState": {
    "@odata.type": "#microsoft.graph.configurationManagerClientHealthState",
    "errorCode": "Int32",
    "lastSyncDateTime": "DateTimeOffset",
    "state": "String"
  },
  "configurationManagerClientInformation": {
    "@odata.type": "#microsoft.graph.configurationManagerClientInformation",
    "clientIdentifier": "String",
    "isBlocked": "Boolean"
  },
  "deviceActionResults": [
    {
      "@odata.type": "#microsoft.graph.deviceActionResult",
      "actionName": "String",
      "actionState": "String",
      "lastUpdatedDateTime": "DateTimeOffset",
      "startDateTime": "DateTimeOffset"
    }
  ],
  "deviceCategoryDisplayName": "String",
  "deviceEnrollmentType": "String",
  "deviceHealthAttestationState": {
    "@odata.type": "#microsoft.graph.deviceHealthAttestationState",
    "attestationIdentityKey": "String",
    "bitLockerStatus": "String",
    "bootAppSecurityVersion": "String",
    "bootDebugging": "String",
    "bootManagerSecurityVersion": "String",
    "bootManagerVersion": "String",
    "bootRevisionListInfo": "String",
    "codeIntegrity": "String",
    "codeIntegrityCheckVersion": "String",
    "codeIntegrityPolicy": "String",
    "contentNamespaceUrl": "String",
    "contentVersion": "String",
    "dataExcutionPolicy": "String",
    "deviceHealthAttestationStatus": "String",
    "earlyLaunchAntiMalwareDriverProtection": "String",
    "healthAttestationSupportedStatus": "String",
    "healthStatusMismatchInfo": "String",
    "issuedDateTime": "DateTimeOffset",
    "lastUpdateDateTime": "String",
    "operatingSystemKernelDebugging": "String",
    "operatingSystemRevListInfo": "String",
    "pcr0": "String",
    "pcrHashAlgorithm": "String",
    "resetCount": "Int64",
    "restartCount": "Int64",
    "safeMode": "String",
    "secureBoot": "String",
    "secureBootConfigurationPolicyFingerPrint": "String",
    "testSigning": "String",
    "tpmVersion": "String",
    "virtualSecureMode": "String",
    "windowsPE": "String"
  },
  "deviceName": "String",
  "deviceRegistrationState": "String",
  "deviceType": "String",
  "easActivated": "Boolean",
  "easActivationDateTime": "DateTimeOffset",
  "easDeviceId": "String",
  "emailAddress": "String",
  "enrolledDateTime": "DateTimeOffset",
  "ethernetMacAddress": "String",
  "exchangeAccessState": "String",
  "exchangeAccessStateReason": "String",
  "exchangeLastSuccessfulSyncDateTime": "DateTimeOffset",
  "freeStorageSpaceInBytes": "Int64",
  "hardwareInformation": {
    "@odata.type": "#microsoft.graph.hardwareInformation",
    "cellularTechnology": "String",
    "deviceFullQualifiedDomainName": "String",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "String",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
    "deviceGuardVirtualizationBasedSecurityState": "String",
    "freeStorageSpace": "Int64",
    "imei": "String",
    "isEncrypted": "Boolean",
    "isSharedDevice": "Boolean",
    "isSupervised": "Boolean",
    "manufacturer": "String",
    "meid": "String",
    "model": "String",
    "operatingSystemEdition": "String",
    "operatingSystemLanguage": "String",
    "operatingSystemProductType": "Int32",
    "osBuildNumber": "String",
    "phoneNumber": "String",
    "serialNumber": "String",
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "#microsoft.graph.sharedAppleDeviceUser",
        "dataQuota": "Int64",
        "dataToSync": "Boolean",
        "dataUsed": "Int64",
        "userPrincipalName": "String"
      }
    ],
    "subscriberCarrier": "String",
    "totalStorageSpace": "Int64",
    "tpmSpecificationVersion": "String",
    "wifiMac": "String"
  },
  "iccid": "String",
  "id": "String(identifier)",
  "imei": "String",
  "isEncrypted": "Boolean",
  "isSupervised": "Boolean",
  "jailBroken": "String",
  "joinType": "String",
  "lastSyncDateTime": "DateTimeOffset",
  "lostModeState": "String",
  "managedDeviceName": "String",
  "managedDeviceOwnerType": "String",
  "managementAgent": "String",
  "managementCertificateExpirationDate": "DateTimeOffset",
  "managementState": "String",
  "manufacturer": "String",
  "meid": "String",
  "model": "String",
  "notes": "String",
  "operatingSystem": "String",
  "osVersion": "String",
  "ownerType": "String",
  "partnerReportedThreatState": "String",
  "phoneNumber": "String",
  "physicalMemoryInBytes": "Int64",
  "preferMdmOverGroupPolicyAppliedDateTime": "DateTimeOffset",
  "processorArchitecture": "String",
  "remoteAssistanceSessionErrorDetails": "String",
  "remoteAssistanceSessionUrl": "String",
  "requireUserEnrollmentApproval": "Boolean",
  "retireAfterDateTime": "DateTimeOffset",
  "roleScopeTagIds": [
    "String"
  ],
  "serialNumber": "String",
  "skuFamily": "String",
  "specificationVersion": "String",
  "subscriberCarrier": "String",
  "totalStorageSpaceInBytes": "Int64",
  "udid": "String",
  "userDisplayName": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "usersLoggedOn": [
    {
      "@odata.type": "#microsoft.graph.loggedOnUser",
      "lastLogOnDateTime": "DateTimeOffset",
      "userId": "String"
    }
  ],
  "wiFiMacAddress": "String",
  "windowsActiveMalwareCount": "Int32",
  "windowsRemediatedMalwareCount": "Int32"
}
}

```