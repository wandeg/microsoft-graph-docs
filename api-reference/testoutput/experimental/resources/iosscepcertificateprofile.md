---
title: "iosScepCertificateProfile resource type"
description: "iOS SCEP certificate profile."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosScepCertificateProfile resource type


Namespace: microsoft.graph

iOS SCEP certificate profile.


Inherits from [iosCertificateProfileBase](../resources/ioscertificateprofilebase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List iosScepCertificateProfiles](../api/iosscepcertificateprofile-list.md)|[iosScepCertificateProfile](../resources/iosscepcertificateprofile.md) collection|List properties and relationships of the [iosScepCertificateProfile](../resources/iosscepcertificateprofile.md) objects.|
|[Get iosScepCertificateProfile](../api/iosscepcertificateprofile-get.md)|[iosScepCertificateProfile](../resources/iosscepcertificateprofile.md)|Read properties and relationships of the [iosScepCertificateProfile](../resources/iosscepcertificateprofile.md) object.|
|[Create iosScepCertificateProfile](../api/iosscepcertificateprofile-create.md)|[iosScepCertificateProfile](../resources/iosscepcertificateprofile.md)|Create a new [iosScepCertificateProfile](../resources/iosscepcertificateprofile.md) object.|
|[Delete iosScepCertificateProfile](../api/iosscepcertificateprofile-delete.md)|None|Deletes a [iosScepCertificateProfile](../resources/iosscepcertificateprofile.md).|
|[Update iosScepCertificateProfile](../api/iosscepcertificateprofile-update.md)|[iosScepCertificateProfile](../resources/iosscepcertificateprofile.md)|Update the properties of a [iosScepCertificateProfile](../resources/iosscepcertificateprofile.md) object.|
|[List groupAssignments](../api/iosscepcertificateprofile-list-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) collection|Get the deviceConfigurationGroupAssignments from the groupAssignments navigation property.|
|[Add groupAssignments](../api/iosscepcertificateprofile-post-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md)|Add groupAssignments by posting to the groupAssignments collection.|
|[List assignments](../api/iosscepcertificateprofile-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|Get the deviceConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/iosscepcertificateprofile-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/iosscepcertificateprofile-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Get the deviceConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/iosscepcertificateprofile-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/iosscepcertificateprofile-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Get the deviceConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/iosscepcertificateprofile-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[Get deviceConfigurationUserOverview](../api/deviceconfigurationuseroverview-get.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Read properties and relationships of the [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/iosscepcertificateprofile-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/iosscepcertificateprofile-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|
|[Get iosTrustedRootCertificate](../api/iostrustedrootcertificate-get.md)|[iosTrustedRootCertificate](../resources/iostrustedrootcertificate.md)|Read properties and relationships of the [iosTrustedRootCertificate](../resources/iostrustedrootcertificate.md) object.|
|[List managedDeviceCertificateStates](../api/iosscepcertificateprofile-list-manageddevicecertificatestates.md)|[managedDeviceCertificateState](../resources/manageddevicecertificatestate.md) collection|Get the managedDeviceCertificateStates from the managedDeviceCertificateStates navigation property.|
|[Create managedDeviceCertificateStates](../api/iosscepcertificateprofile-post-manageddevicecertificatestates.md)|[managedDeviceCertificateState](../resources/manageddevicecertificatestate.md)|Create managedDeviceCertificateStates by posting to the managedDeviceCertificateStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|certificateStore|Enumeration|Target store certificate. Possible values are: `user`, `machine`.|
|certificateValidityPeriodScale|Enumeration|Scale for the Certificate Validity Period. Inherited from [iosCertificateProfileBase](../resources/ioscertificateprofilebase.md). Possible values are: `days`, `months`, `years`.|
|certificateValidityPeriodValue|Int32|Value for the Certificate Validity Period. Inherited from [iosCertificateProfileBase](../resources/ioscertificateprofilebase.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|customSubjectAlternativeNames|[customSubjectAlternativeName](../resources/customsubjectalternativename.md) collection|Custom Subject Alternative Name Settings. The OnPremisesUserPrincipalName variable is support as well as others documented here: http://go.microsoft.com/fwlink/?LinkId=2027630. This collection can contain a maximum of 500 elements.|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/devicemanagementapplicabilityruledevicemode.md)|The device mode applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/devicemanagementapplicabilityruleosedition.md)|The OS edition applicability for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/devicemanagementapplicabilityruleosversion.md)|The OS version applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|extendedKeyUsages|[extendedKeyUsage](../resources/extendedkeyusage.md) collection|Extended Key Usage (EKU) settings. This collection can contain a maximum of 500 elements.|
|id|String| Inherited from [entity](../resources/entity.md)|
|keySize|Enumeration|SCEP Key Size. Possible values are: `size1024`, `size2048`.|
|keyUsage|Enumeration|SCEP Key Usage. Possible values are: `keyEncipherment`, `digitalSignature`.|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|renewalThresholdPercentage|Int32|Certificate renewal threshold percentage. Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/ioscertificateprofilebase.md)|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|scepServerUrls|String collection|SCEP Server Url(s).|
|subjectAlternativeNameFormatString|String|Custom String that defines the AAD Attribute.|
|subjectAlternativeNameType|Enumeration|Certificate Subject Alternative Name type. Inherited from [iosCertificateProfileBase](../resources/ioscertificateprofilebase.md). Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.|
|subjectNameFormat|Enumeration|Certificate Subject Name Format. Inherited from [iosCertificateProfileBase](../resources/ioscertificateprofilebase.md). Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.|
|subjectNameFormatString|String|Custom format to use with SubjectNameFormat = Custom. Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US|
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
|rootCertificate|[iosTrustedRootCertificate](../resources/iostrustedrootcertificate.md)|Trusted Root Certificate.|
|userStatuses|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Device configuration installation status by user. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosScepCertificateProfile",
  "baseType": "microsoft.graph.iosCertificateProfileBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
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
  "scepServerUrls": [
    "String"
  ],
  "subjectNameFormatString": "String",
  "keyUsage": "String",
  "keySize": "String",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "objectIdentifier": "String"
    }
  ],
  "subjectAlternativeNameFormatString": "String",
  "certificateStore": "String",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "String"
    }
  ]
}
```

