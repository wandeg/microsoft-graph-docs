---
title: "windowsPhone81SCEPCertificateProfile resource type"
description: "Windows Phone 8.1+ SCEP certificate profile"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# windowsPhone81SCEPCertificateProfile resource type

Windows Phone 8.1+ SCEP certificate profile


Inherits from [windowsPhone81CertificateProfileBase](../resources/windowsPhone81CertificateProfileBase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windowsPhone81SCEPCertificateProfiles](../api/windowsphone81scepcertificateprofile-list.md)|[windowsPhone81SCEPCertificateProfile](../resources/windowsPhone81SCEPCertificateProfile.md) collection|List properties and relationships of the [windowsPhone81SCEPCertificateProfile](../resources/windowsphone81scepcertificateprofile.md) objects.|
|[Get windowsPhone81SCEPCertificateProfile](../api/windowsphone81scepcertificateprofile-get.md)|[windowsPhone81SCEPCertificateProfile](../resources/windowsPhone81SCEPCertificateProfile.md)|Read properties and relationships of the [windowsPhone81SCEPCertificateProfile](../resources/windowsphone81scepcertificateprofile.md) object.|
|[Create windowsPhone81SCEPCertificateProfile](../api/windowsphone81scepcertificateprofile-create.md)|[windowsPhone81SCEPCertificateProfile](../resources/windowsPhone81SCEPCertificateProfile.md)|Create a new [windowsPhone81SCEPCertificateProfile](../resources/windowsphone81scepcertificateprofile.md) object.|
|[Delete windowsPhone81SCEPCertificateProfile](../api/windowsphone81scepcertificateprofile-delete.md)|None|Deletes a [windowsPhone81SCEPCertificateProfile](../resources/windowsphone81scepcertificateprofile.md).|
|[Update windowsPhone81SCEPCertificateProfile](../api/windowsphone81scepcertificateprofile-update.md)|[windowsPhone81SCEPCertificateProfile](../resources/windowsPhone81SCEPCertificateProfile.md)|Update the properties of a [windowsPhone81SCEPCertificateProfile](../resources/windowsphone81scepcertificateprofile.md) object.|
|[List groupAssignments](../api/windowsphone81scepcertificateprofile-list-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceConfigurationGroupAssignment.md) collection|Get the deviceConfigurationGroupAssignments from the groupAssignments navigation property.|
|[Add groupAssignments](../api/windowsphone81scepcertificateprofile-post-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceConfigurationGroupAssignment.md)|Add groupAssignments by posting to the groupAssignments collection.|
|[List assignments](../api/windowsphone81scepcertificateprofile-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceConfigurationAssignment.md) collection|Get the deviceConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/windowsphone81scepcertificateprofile-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceConfigurationAssignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/windowsphone81scepcertificateprofile-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceConfigurationDeviceStatus.md) collection|Get the deviceConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/windowsphone81scepcertificateprofile-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceConfigurationDeviceStatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/windowsphone81scepcertificateprofile-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceConfigurationUserStatus.md) collection|Get the deviceConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/windowsphone81scepcertificateprofile-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceConfigurationUserStatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/deviceConfigurationDeviceOverview.md)|Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[Get deviceConfigurationUserOverview](../api/deviceconfigurationuseroverview-get.md)|[deviceConfigurationUserOverview](../resources/deviceConfigurationUserOverview.md)|Read properties and relationships of the [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/windowsphone81scepcertificateprofile-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/windowsphone81scepcertificateprofile-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|
|[Get windowsPhone81TrustedRootCertificate](../api/windowsphone81trustedrootcertificate-get.md)|[windowsPhone81TrustedRootCertificate](../resources/windowsPhone81TrustedRootCertificate.md)|Read properties and relationships of the [windowsPhone81TrustedRootCertificate](../resources/windowsphone81trustedrootcertificate.md) object.|
|[List managedDeviceCertificateStates](../api/windowsphone81scepcertificateprofile-list-manageddevicecertificatestates.md)|[managedDeviceCertificateState](../resources/managedDeviceCertificateState.md) collection|Get the managedDeviceCertificateStates from the managedDeviceCertificateStates navigation property.|
|[Create managedDeviceCertificateStates](../api/windowsphone81scepcertificateprofile-post-manageddevicecertificatestates.md)|[managedDeviceCertificateState](../resources/managedDeviceCertificateState.md)|Create managedDeviceCertificateStates by posting to the managedDeviceCertificateStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|certificateValidityPeriodScale|Enumeration|Scale for the Certificate Validity Period. Inherited from [windowsPhone81CertificateProfileBase](../resources/windowsPhone81CertificateProfileBase.md). Possible values are: `days`, `months`, `years`.|
|certificateValidityPeriodValue|Int32|Value for the Certificate Validtiy Period. Inherited from [windowsPhone81CertificateProfileBase](../resources/windowsPhone81CertificateProfileBase.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/deviceManagementApplicabilityRuleDeviceMode.md)|The device mode applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/deviceManagementApplicabilityRuleOsEdition.md)|The OS edition applicability for this Policy. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/deviceManagementApplicabilityRuleOsVersion.md)|The OS version applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|extendedKeyUsages|[extendedKeyUsage](../resources/extendedKeyUsage.md) collection|Extended Key Usage (EKU) settings. This collection can contain a maximum of 500 elements. Inherited from [windowsPhone81CertificateProfileBase](../resources/windowsPhone81CertificateProfileBase.md)|
|hashAlgorithm|Enumeration|SCEP Hash Algorithm. Possible values are: `sha1`, `sha2`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|keySize|Enumeration|SCEP Key Size. Possible values are: `size1024`, `size2048`.|
|keyStorageProvider|Enumeration|Key Storage Provider (KSP). Inherited from [windowsPhone81CertificateProfileBase](../resources/windowsPhone81CertificateProfileBase.md). Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.|
|keyUsage|Enumeration|SCEP Key Usage. Possible values are: `keyEncipherment`, `digitalSignature`.|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|renewalThresholdPercentage|Int32|Certificate renewal threshold percentage. Inherited from [windowsPhone81CertificateProfileBase](../resources/windowsPhone81CertificateProfileBase.md)|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|scepServerUrls|String collection|SCEP Server Url(s).|
|subjectAlternativeNameFormatString|String|Custom String that defines the AAD Attribute.|
|subjectAlternativeNameType|Enumeration|Certificate Subject Alternative Name Type. Inherited from [windowsPhone81CertificateProfileBase](../resources/windowsPhone81CertificateProfileBase.md). Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.|
|subjectNameFormat|Enumeration|Certificate Subject Name Format. Inherited from [windowsPhone81CertificateProfileBase](../resources/windowsPhone81CertificateProfileBase.md). Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
|subjectNameFormatString|String|Custom format to use with SubjectNameFormat = Custom. Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US|
|supportsScopeTags|Boolean|Indicates whether or not the underlying Device Configuration supports the assignment of scope tags. Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users. This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal. This property is read-only. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/deviceConfigurationAssignment.md) collection|The list of assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md) collection|Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/deviceConfigurationDeviceStatus.md) collection|Device configuration installation status by device. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/deviceConfigurationDeviceOverview.md)|Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/deviceConfigurationGroupAssignment.md) collection|The list of group assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|managedDeviceCertificateStates|[managedDeviceCertificateState](../resources/managedDeviceCertificateState.md) collection|Certificate state for devices|
|rootCertificate|[windowsPhone81TrustedRootCertificate](../resources/windowsPhone81TrustedRootCertificate.md)|Trusted Root Certificate.|
|userStatuses|[deviceConfigurationUserStatus](../resources/deviceConfigurationUserStatus.md) collection|Device configuration installation status by user. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/deviceConfigurationUserOverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPhone81SCEPCertificateProfile",
  "baseType": "microsoft.graph.windowsPhone81CertificateProfileBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "renewalThresholdPercentage": 1024,
  "keyStorageProvider": "String",
  "subjectNameFormat": "String",
  "subjectAlternativeNameType": "String",
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "objectIdentifier": "String"
    }
  ],
  "scepServerUrls": [
    "String"
  ],
  "subjectNameFormatString": "String",
  "keyUsage": "String",
  "keySize": "String",
  "hashAlgorithm": "String",
  "subjectAlternativeNameFormatString": "String"
}
```

