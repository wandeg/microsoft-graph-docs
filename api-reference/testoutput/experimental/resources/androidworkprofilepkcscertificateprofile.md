---
title: "androidWorkProfilePkcsCertificateProfile resource type"
description: "Android Work Profile PKCS certificate profile"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# androidWorkProfilePkcsCertificateProfile resource type


Namespace: microsoft.graph

Android Work Profile PKCS certificate profile


Inherits from [androidWorkProfileCertificateProfileBase](../resources/androidworkprofilecertificateprofilebase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List androidWorkProfilePkcsCertificateProfiles](../api/androidworkprofilepkcscertificateprofile-list.md)|[androidWorkProfilePkcsCertificateProfile](../resources/androidworkprofilepkcscertificateprofile.md) collection|List properties and relationships of the [androidWorkProfilePkcsCertificateProfile](../resources/androidworkprofilepkcscertificateprofile.md) objects.|
|[Get androidWorkProfilePkcsCertificateProfile](../api/androidworkprofilepkcscertificateprofile-get.md)|[androidWorkProfilePkcsCertificateProfile](../resources/androidworkprofilepkcscertificateprofile.md)|Read properties and relationships of the [androidWorkProfilePkcsCertificateProfile](../resources/androidworkprofilepkcscertificateprofile.md) object.|
|[Create androidWorkProfilePkcsCertificateProfile](../api/androidworkprofilepkcscertificateprofile-create.md)|[androidWorkProfilePkcsCertificateProfile](../resources/androidworkprofilepkcscertificateprofile.md)|Create a new [androidWorkProfilePkcsCertificateProfile](../resources/androidworkprofilepkcscertificateprofile.md) object.|
|[Delete androidWorkProfilePkcsCertificateProfile](../api/androidworkprofilepkcscertificateprofile-delete.md)|None|Deletes a [androidWorkProfilePkcsCertificateProfile](../resources/androidworkprofilepkcscertificateprofile.md).|
|[Update androidWorkProfilePkcsCertificateProfile](../api/androidworkprofilepkcscertificateprofile-update.md)|[androidWorkProfilePkcsCertificateProfile](../resources/androidworkprofilepkcscertificateprofile.md)|Update the properties of a [androidWorkProfilePkcsCertificateProfile](../resources/androidworkprofilepkcscertificateprofile.md) object.|
|[List groupAssignments](../api/androidworkprofilepkcscertificateprofile-list-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) collection|Get the deviceConfigurationGroupAssignments from the groupAssignments navigation property.|
|[Add groupAssignments](../api/androidworkprofilepkcscertificateprofile-post-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md)|Add groupAssignments by posting to the groupAssignments collection.|
|[List assignments](../api/androidworkprofilepkcscertificateprofile-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|Get the deviceConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/androidworkprofilepkcscertificateprofile-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/androidworkprofilepkcscertificateprofile-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Get the deviceConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/androidworkprofilepkcscertificateprofile-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/androidworkprofilepkcscertificateprofile-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Get the deviceConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/androidworkprofilepkcscertificateprofile-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[Get deviceConfigurationUserOverview](../api/deviceconfigurationuseroverview-get.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Read properties and relationships of the [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/androidworkprofilepkcscertificateprofile-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/androidworkprofilepkcscertificateprofile-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|
|[Get androidWorkProfileTrustedRootCertificate](../api/androidworkprofiletrustedrootcertificate-get.md)|[androidWorkProfileTrustedRootCertificate](../resources/androidworkprofiletrustedrootcertificate.md)|Read properties and relationships of the [androidWorkProfileTrustedRootCertificate](../resources/androidworkprofiletrustedrootcertificate.md) object.|
|[List managedDeviceCertificateStates](../api/androidworkprofilepkcscertificateprofile-list-manageddevicecertificatestates.md)|[managedDeviceCertificateState](../resources/manageddevicecertificatestate.md) collection|Get the managedDeviceCertificateStates from the managedDeviceCertificateStates navigation property.|
|[Create managedDeviceCertificateStates](../api/androidworkprofilepkcscertificateprofile-post-manageddevicecertificatestates.md)|[managedDeviceCertificateState](../resources/manageddevicecertificatestate.md)|Create managedDeviceCertificateStates by posting to the managedDeviceCertificateStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|certificateStore|Enumeration|Target store certificate. Possible values are: `user`, `machine`.|
|certificateTemplateName|String|PKCS Certificate Template Name|
|certificateValidityPeriodScale|Enumeration|Scale for the Certificate Validity Period. Inherited from [androidWorkProfileCertificateProfileBase](../resources/androidworkprofilecertificateprofilebase.md). Possible values are: `days`, `months`, `years`.|
|certificateValidityPeriodValue|Int32|Value for the Certificate Validity Period. Inherited from [androidWorkProfileCertificateProfileBase](../resources/androidworkprofilecertificateprofilebase.md)|
|certificationAuthority|String|PKCS Certification Authority|
|certificationAuthorityName|String|PKCS Certification Authority Name|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|customSubjectAlternativeNames|[customSubjectAlternativeName](../resources/customsubjectalternativename.md) collection|Custom Subject Alternative Name Settings. This collection can contain a maximum of 500 elements.|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/devicemanagementapplicabilityruledevicemode.md)|The device mode applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/devicemanagementapplicabilityruleosedition.md)|The OS edition applicability for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/devicemanagementapplicabilityruleosversion.md)|The OS version applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|extendedKeyUsages|[extendedKeyUsage](../resources/extendedkeyusage.md) collection|Extended Key Usage (EKU) settings. This collection can contain a maximum of 500 elements. Inherited from [androidWorkProfileCertificateProfileBase](../resources/androidworkprofilecertificateprofilebase.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|renewalThresholdPercentage|Int32|Certificate renewal threshold percentage. Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/androidworkprofilecertificateprofilebase.md)|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|subjectAlternativeNameFormatString|String|Custom String that defines the AAD Attribute.|
|subjectAlternativeNameType|Enumeration|Certificate Subject Alternative Name Type. Inherited from [androidWorkProfileCertificateProfileBase](../resources/androidworkprofilecertificateprofilebase.md). Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.|
|subjectNameFormat|Enumeration|Certificate Subject Name Format. Inherited from [androidWorkProfileCertificateProfileBase](../resources/androidworkprofilecertificateprofilebase.md). Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
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
|rootCertificate|[androidWorkProfileTrustedRootCertificate](../resources/androidworkprofiletrustedrootcertificate.md)|Trusted Root Certificate. Inherited from [androidWorkProfileCertificateProfileBase](../resources/androidworkprofilecertificateprofilebase.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Device configuration installation status by user. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidWorkProfilePkcsCertificateProfile",
  "baseType": "microsoft.graph.androidWorkProfileCertificateProfileBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
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
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "objectIdentifier": "String"
    }
  ],
  "subjectAlternativeNameType": "String",
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
  "certificateTemplateName": "String",
  "subjectAlternativeNameFormatString": "String",
  "subjectNameFormatString": "String",
  "certificateStore": "String",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "String"
    }
  ]
}
```

