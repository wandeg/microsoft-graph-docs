---
title: "iosEasEmailProfileConfiguration resource type"
description: "By providing configurations in this profile you can instruct the native email client on iOS devices to communicate with an Exchange server and get email, contacts, calendar, reminders, and notes. Furthermore, you can also specify how much email to sync and how often the device should sync."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosEasEmailProfileConfiguration resource type


Namespace: microsoft.graph

By providing configurations in this profile you can instruct the native email client on iOS devices to communicate with an Exchange server and get email, contacts, calendar, reminders, and notes. Furthermore, you can also specify how much email to sync and how often the device should sync.


Inherits from [easEmailProfileConfigurationBase](../resources/easemailprofileconfigurationbase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List iosEasEmailProfileConfigurations](../api/ioseasemailprofileconfiguration-list.md)|[iosEasEmailProfileConfiguration](../resources/ioseasemailprofileconfiguration.md) collection|List properties and relationships of the [iosEasEmailProfileConfiguration](../resources/ioseasemailprofileconfiguration.md) objects.|
|[Get iosEasEmailProfileConfiguration](../api/ioseasemailprofileconfiguration-get.md)|[iosEasEmailProfileConfiguration](../resources/ioseasemailprofileconfiguration.md)|Read properties and relationships of the [iosEasEmailProfileConfiguration](../resources/ioseasemailprofileconfiguration.md) object.|
|[Create iosEasEmailProfileConfiguration](../api/ioseasemailprofileconfiguration-create.md)|[iosEasEmailProfileConfiguration](../resources/ioseasemailprofileconfiguration.md)|Create a new [iosEasEmailProfileConfiguration](../resources/ioseasemailprofileconfiguration.md) object.|
|[Delete iosEasEmailProfileConfiguration](../api/ioseasemailprofileconfiguration-delete.md)|None|Deletes a [iosEasEmailProfileConfiguration](../resources/ioseasemailprofileconfiguration.md).|
|[Update iosEasEmailProfileConfiguration](../api/ioseasemailprofileconfiguration-update.md)|[iosEasEmailProfileConfiguration](../resources/ioseasemailprofileconfiguration.md)|Update the properties of a [iosEasEmailProfileConfiguration](../resources/ioseasemailprofileconfiguration.md) object.|
|[List groupAssignments](../api/ioseasemailprofileconfiguration-list-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) collection|Get the deviceConfigurationGroupAssignments from the groupAssignments navigation property.|
|[Add groupAssignments](../api/ioseasemailprofileconfiguration-post-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md)|Add groupAssignments by posting to the groupAssignments collection.|
|[List assignments](../api/ioseasemailprofileconfiguration-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|Get the deviceConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/ioseasemailprofileconfiguration-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/ioseasemailprofileconfiguration-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Get the deviceConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/ioseasemailprofileconfiguration-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/ioseasemailprofileconfiguration-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Get the deviceConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/ioseasemailprofileconfiguration-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[Get deviceConfigurationUserOverview](../api/deviceconfigurationuseroverview-get.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Read properties and relationships of the [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/ioseasemailprofileconfiguration-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/ioseasemailprofileconfiguration-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|
|[Get iosCertificateProfileBase](../api/ioscertificateprofilebase-get.md)|[iosCertificateProfileBase](../resources/ioscertificateprofilebase.md)|Read properties and relationships of the [iosCertificateProfileBase](../resources/ioscertificateprofilebase.md) object.|
|[Get iosCertificateProfile](../api/ioscertificateprofile-get.md)|[iosCertificateProfile](../resources/ioscertificateprofile.md)|Read properties and relationships of the [iosCertificateProfile](../resources/ioscertificateprofile.md) object.|
|[Get iosCertificateProfile](../api/ioscertificateprofile-get.md)|[iosCertificateProfile](../resources/ioscertificateprofile.md)|Read properties and relationships of the [iosCertificateProfile](../resources/ioscertificateprofile.md) object.|
|[Get deviceManagementDerivedCredentialSettings](../api/devicemanagementderivedcredentialsettings-get.md)|[deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md)|Read properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountName|String|Account name.|
|authenticationMethod|Enumeration|Authentication method for this Email profile. Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.|
|blockMovingMessagesToOtherEmailAccounts|Boolean|Indicates whether or not to block moving messages to other email accounts.|
|blockSendingEmailFromThirdPartyApps|Boolean|Indicates whether or not to block sending email from third party apps.|
|blockSyncingRecentlyUsedEmailAddresses|Boolean|Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|customDomainName|String|Custom domain name value used while generating an email profile before installing on the device. Inherited from [easEmailProfileConfigurationBase](../resources/easemailprofileconfigurationbase.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/devicemanagementapplicabilityruledevicemode.md)|The device mode applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/devicemanagementapplicabilityruleosedition.md)|The OS edition applicability for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/devicemanagementapplicabilityruleosversion.md)|The OS version applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|durationOfEmailToSync|Enumeration|Duration of time email should be synced back to. . Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.|
|easServices|Enumeration|Exchange data to sync. Possible values are: `none`, `calendars`, `contacts`, `email`, `notes`, `reminders`.|
|easServicesUserOverrideEnabled|Boolean|Allow users to change sync settings.|
|emailAddressSource|Enumeration|Email attribute that is picked from AAD and injected into this profile before installing on the device. Possible values are: `userPrincipalName`, `primarySmtpAddress`.|
|encryptionCertificateType|Enumeration|Encryption Certificate type for this Email profile. Possible values are: `none`, `certificate`, `derivedCredential`.|
|hostName|String|Exchange location that (URL) that the native mail app connects to.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|requireSmime|Boolean|Indicates whether or not to use S/MIME certificate.|
|requireSsl|Boolean|Indicates whether or not to use SSL.|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|signingCertificateType|Enumeration|Signing Certificate type for this Email profile. Possible values are: `none`, `certificate`, `derivedCredential`.|
|smimeEnablePerMessageSwitch|Boolean|Indicates whether or not to allow unencrypted emails.|
|smimeEncryptByDefaultEnabled|Boolean|If set to true S/MIME encryption is enabled by default.|
|smimeEncryptByDefaultUserOverrideEnabled|Boolean|If set to true, the user can toggle the encryption by default setting.|
|smimeEncryptionCertificateUserOverrideEnabled|Boolean|If set to true the user can select the S/MIME encryption identity. |
|smimeSigningCertificateUserOverrideEnabled|Boolean|If set to true, the user can select the signing identity.|
|smimeSigningEnabled|Boolean|If set to true S/MIME signing is enabled for this account|
|smimeSigningUserOverrideEnabled|Boolean|If set to true, the user can toggle S/MIME signing on or off.|
|supportsScopeTags|Boolean|Indicates whether or not the underlying Device Configuration supports the assignment of scope tags. Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users. This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal. This property is read-only. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|useOAuth|Boolean|Specifies whether the connection should use OAuth for authentication.|
|userDomainNameSource|Enumeration|UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device. Inherited from [easEmailProfileConfigurationBase](../resources/easemailprofileconfigurationbase.md). Possible values are: `fullDomainName`, `netBiosDomainName`.|
|usernameAADSource|Enumeration|Name of the AAD field, that will be used to retrieve UserName for email profile. Inherited from [easEmailProfileConfigurationBase](../resources/easemailprofileconfigurationbase.md). Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.|
|usernameSource|Enumeration|Username attribute that is picked from AAD and injected into this profile before installing on the device. Inherited from [easEmailProfileConfigurationBase](../resources/easemailprofileconfigurationbase.md). Possible values are: `userPrincipalName`, `primarySmtpAddress`.|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|The list of assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|derivedCredentialSettings|[deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md)|Tenant level settings for the Derived Credentials to be used for authentication.|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Device configuration installation status by device. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) collection|The list of group assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|identityCertificate|[iosCertificateProfileBase](../resources/ioscertificateprofilebase.md)|Identity certificate.|
|smimeEncryptionCertificate|[iosCertificateProfile](../resources/ioscertificateprofile.md)|S/MIME encryption certificate.|
|smimeSigningCertificate|[iosCertificateProfile](../resources/ioscertificateprofile.md)|S/MIME signing certificate.|
|userStatuses|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Device configuration installation status by user. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosEasEmailProfileConfiguration",
  "baseType": "microsoft.graph.easEmailProfileConfigurationBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
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
  "usernameSource": "String",
  "usernameAADSource": "String",
  "userDomainNameSource": "String",
  "customDomainName": "String",
  "accountName": "String",
  "authenticationMethod": "String",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "String",
  "emailAddressSource": "String",
  "easServices": "String",
  "easServicesUserOverrideEnabled": true,
  "hostName": "String",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "smimeEncryptByDefaultEnabled": true,
  "smimeSigningEnabled": true,
  "smimeSigningUserOverrideEnabled": true,
  "smimeEncryptByDefaultUserOverrideEnabled": true,
  "smimeSigningCertificateUserOverrideEnabled": true,
  "smimeEncryptionCertificateUserOverrideEnabled": true,
  "requireSsl": true,
  "useOAuth": true,
  "signingCertificateType": "String",
  "encryptionCertificateType": "String"
}
```

