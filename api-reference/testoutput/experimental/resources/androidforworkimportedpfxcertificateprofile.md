---
title: "androidForWorkImportedPFXCertificateProfile resource type"
description: "Android For Work PFX Import certificate profile"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# androidForWorkImportedPFXCertificateProfile resource type


Namespace: microsoft.graph

Android For Work PFX Import certificate profile


Inherits from [androidCertificateProfileBase](../resources/androidcertificateprofilebase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List androidForWorkImportedPFXCertificateProfiles](../api/androidforworkimportedpfxcertificateprofile-list.md)|[androidForWorkImportedPFXCertificateProfile](../resources/androidforworkimportedpfxcertificateprofile.md) collection|List properties and relationships of the [androidForWorkImportedPFXCertificateProfile](../resources/androidforworkimportedpfxcertificateprofile.md) objects.|
|[Get androidForWorkImportedPFXCertificateProfile](../api/androidforworkimportedpfxcertificateprofile-get.md)|[androidForWorkImportedPFXCertificateProfile](../resources/androidforworkimportedpfxcertificateprofile.md)|Read properties and relationships of the [androidForWorkImportedPFXCertificateProfile](../resources/androidforworkimportedpfxcertificateprofile.md) object.|
|[Create androidForWorkImportedPFXCertificateProfile](../api/androidforworkimportedpfxcertificateprofile-create.md)|[androidForWorkImportedPFXCertificateProfile](../resources/androidforworkimportedpfxcertificateprofile.md)|Create a new [androidForWorkImportedPFXCertificateProfile](../resources/androidforworkimportedpfxcertificateprofile.md) object.|
|[Delete androidForWorkImportedPFXCertificateProfile](../api/androidforworkimportedpfxcertificateprofile-delete.md)|None|Deletes a [androidForWorkImportedPFXCertificateProfile](../resources/androidforworkimportedpfxcertificateprofile.md).|
|[Update androidForWorkImportedPFXCertificateProfile](../api/androidforworkimportedpfxcertificateprofile-update.md)|[androidForWorkImportedPFXCertificateProfile](../resources/androidforworkimportedpfxcertificateprofile.md)|Update the properties of a [androidForWorkImportedPFXCertificateProfile](../resources/androidforworkimportedpfxcertificateprofile.md) object.|
|[List groupAssignments](../api/androidforworkimportedpfxcertificateprofile-list-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) collection|Get the deviceConfigurationGroupAssignments from the groupAssignments navigation property.|
|[Add groupAssignments](../api/androidforworkimportedpfxcertificateprofile-post-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md)|Add groupAssignments by posting to the groupAssignments collection.|
|[List assignments](../api/androidforworkimportedpfxcertificateprofile-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|Get the deviceConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/androidforworkimportedpfxcertificateprofile-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/androidforworkimportedpfxcertificateprofile-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Get the deviceConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/androidforworkimportedpfxcertificateprofile-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/androidforworkimportedpfxcertificateprofile-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Get the deviceConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/androidforworkimportedpfxcertificateprofile-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[Get deviceConfigurationUserOverview](../api/deviceconfigurationuseroverview-get.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Read properties and relationships of the [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/androidforworkimportedpfxcertificateprofile-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/androidforworkimportedpfxcertificateprofile-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|
|[Get androidTrustedRootCertificate](../api/androidtrustedrootcertificate-get.md)|[androidTrustedRootCertificate](../resources/androidtrustedrootcertificate.md)|Read properties and relationships of the [androidTrustedRootCertificate](../resources/androidtrustedrootcertificate.md) object.|
|[List managedDeviceCertificateStates](../api/androidforworkimportedpfxcertificateprofile-list-manageddevicecertificatestates.md)|[managedDeviceCertificateState](../resources/manageddevicecertificatestate.md) collection|Get the managedDeviceCertificateStates from the managedDeviceCertificateStates navigation property.|
|[Create managedDeviceCertificateStates](../api/androidforworkimportedpfxcertificateprofile-post-manageddevicecertificatestates.md)|[managedDeviceCertificateState](../resources/manageddevicecertificatestate.md)|Create managedDeviceCertificateStates by posting to the managedDeviceCertificateStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|certificateValidityPeriodScale|Enumeration|Scale for the Certificate Validity Period. Inherited from [androidCertificateProfileBase](../resources/androidcertificateprofilebase.md). Possible values are: `days`, `months`, `years`.|
|certificateValidityPeriodValue|Int32|Value for the Certificate Validity Period. Inherited from [androidCertificateProfileBase](../resources/androidcertificateprofilebase.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/devicemanagementapplicabilityruledevicemode.md)|The device mode applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/devicemanagementapplicabilityruleosedition.md)|The OS edition applicability for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/devicemanagementapplicabilityruleosversion.md)|The OS version applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|extendedKeyUsages|[extendedKeyUsage](../resources/extendedkeyusage.md) collection|Extended Key Usage (EKU) settings. This collection can contain a maximum of 500 elements. Inherited from [androidCertificateProfileBase](../resources/androidcertificateprofilebase.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|intendedPurpose|Enumeration|Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|renewalThresholdPercentage|Int32|Certificate renewal threshold percentage. Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/androidcertificateprofilebase.md)|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|subjectAlternativeNameType|Enumeration|Certificate Subject Alternative Name Type. Inherited from [androidCertificateProfileBase](../resources/androidcertificateprofilebase.md). Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.|
|subjectNameFormat|Enumeration|Certificate Subject Name Format. Inherited from [androidCertificateProfileBase](../resources/androidcertificateprofilebase.md). Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
|supportsScopeTags|Boolean|Indicates whether or not the underlying Device Configuration supports the assignment of scope tags. Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users. This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal. This property is read-only. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|The list of assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Device configuration installation status by device. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) collection|The list of group assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|managedDeviceCertificateStates|[managedDeviceCertificateState](../resources/manageddevicecertificatestate.md) collection|Certificate state for devices|
|rootCertificate|[androidTrustedRootCertificate](../resources/androidtrustedrootcertificate.md)|Trusted Root Certificate. Inherited from [androidCertificateProfileBase](../resources/androidcertificateprofilebase.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Device configuration installation status by user. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkImportedPFXCertificateProfile",
  "baseType": "microsoft.graph.androidCertificateProfileBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkImportedPFXCertificateProfile",
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
  "intendedPurpose": "String"
}
```

