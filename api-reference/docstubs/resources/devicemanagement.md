---
title: "deviceManagement resource type"
description: "Singleton entity that acts as a container for Android for Work settings functionality under device management."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagement resource type


Namespace: microsoft.graph

Singleton entity that acts as a container for Android for Work settings functionality under device management.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagement](../api/devicemanagement-get.md)|[deviceManagement](../resources/devicemanagement.md)|Read the properties and relationships of a [deviceManagement](../resources/devicemanagement.md) object.|
|[Update deviceManagement](../api/devicemanagement-update.md)|[deviceManagement](../resources/devicemanagement.md)|Update the properties of a [deviceManagement](../resources/devicemanagement.md) object.|
|[enableLegacyPcManagement](../api/devicemanagement-enablelegacypcmanagement.md)|None|**TODO: Add Description**|
|[enableAndroidDeviceAdministratorEnrollment](../api/devicemanagement-enableandroiddeviceadministratorenrollment.md)|None|**TODO: Add Description**|
|[verifyWindowsEnrollmentAutoDiscovery](../api/devicemanagement-verifywindowsenrollmentautodiscovery.md)|Boolean|**TODO: Add Description**|
|[sendCustomNotificationToCompanyPortal](../api/devicemanagement-sendcustomnotificationtocompanyportal.md)|None|**TODO: Add Description**|
|[getEffectivePermissions](../api/devicemanagement-geteffectivepermissions.md)|String collection|**TODO: Add Description**|
|[getEffectivePermissions](../api/devicemanagement-geteffectivepermissions.md)|[rolePermission](../resources/rolepermission.md) collection|**TODO: Add Description**|
|[getRoleScopeTagsByResource](../api/devicemanagement-getrolescopetagsbyresource.md)|[roleScopeTag](../resources/rolescopetag.md) collection|**TODO: Add Description**|
|[getRoleScopeTagsByIds](../api/devicemanagement-getrolescopetagsbyids.md)|[roleScopeTag](../resources/rolescopetag.md) collection|**TODO: Add Description**|
|[getAssignedRoleDetails](../api/devicemanagement-getassignedroledetails.md)|[deviceAndAppManagementAssignedRoleDetails](../resources/deviceandappmanagementassignedroledetails.md)|**TODO: Add Description**|
|[scopedForResource](../api/devicemanagement-scopedforresource.md)|Boolean|**TODO: Add Description**|
|[List auditEvents](../api/devicemanagement-list-auditevents.md)|[auditEvent](../resources/auditevent.md) collection|Get the auditEvents from the auditEvents navigation property.|
|[Create auditEvents](../api/devicemanagement-post-auditevents.md)|[auditEvent](../resources/auditevent.md)|Create a new auditEvents object.|
|[Delete auditEvents](../api/devicemanagement-delete-auditevents.md)|None|Delete an [auditEvent](../resources/auditevent.md) object.|
|[Update auditEvents](../api/devicemanagement-update-auditevents.md)|[auditEvent](../resources/auditevent.md)|Update the properties of an auditEvents object.|
|[Get auditEvent](../api/auditevent-get.md)|[auditEvent](../resources/auditevent.md)|Read the properties and relationships of an [auditEvent](../resources/auditevent.md) object.|
|[List androidForWorkSettings](../api/devicemanagement-list-androidforworksettings.md)|[androidForWorkSettings](../resources/androidforworksettings.md) collection|Get the androidForWorkSettings from the androidForWorkSettings navigation property.|
|[Create androidForWorkSettings](../api/devicemanagement-post-androidforworksettings.md)|[androidForWorkSettings](../resources/androidforworksettings.md)|Create a new androidForWorkSettings object.|
|[Delete androidForWorkSettings](../api/devicemanagement-delete-androidforworksettings.md)|None|Delete an [androidForWorkSettings](../resources/androidforworksettings.md) object.|
|[Update androidForWorkSettings](../api/devicemanagement-update-androidforworksettings.md)|[androidForWorkSettings](../resources/androidforworksettings.md)|Update the properties of an androidForWorkSettings object.|
|[Get androidForWorkSettings](../api/androidforworksettings-get.md)|[androidForWorkSettings](../resources/androidforworksettings.md)|Read the properties and relationships of an [androidForWorkSettings](../resources/androidforworksettings.md) object.|
|[List androidForWorkAppConfigurationSchemas](../api/devicemanagement-list-androidforworkappconfigurationschemas.md)|[androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md) collection|Get the androidForWorkAppConfigurationSchemas from the androidForWorkAppConfigurationSchemas navigation property.|
|[Create androidForWorkAppConfigurationSchemas](../api/devicemanagement-post-androidforworkappconfigurationschemas.md)|[androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md)|Create a new androidForWorkAppConfigurationSchemas object.|
|[Delete androidForWorkAppConfigurationSchemas](../api/devicemanagement-delete-androidforworkappconfigurationschemas.md)|None|Delete an [androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md) object.|
|[Update androidForWorkAppConfigurationSchemas](../api/devicemanagement-update-androidforworkappconfigurationschemas.md)|[androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md)|Update the properties of an androidForWorkAppConfigurationSchemas object.|
|[Get androidForWorkAppConfigurationSchema](../api/androidforworkappconfigurationschema-get.md)|[androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md)|Read the properties and relationships of an [androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md) object.|
|[List androidForWorkEnrollmentProfiles](../api/devicemanagement-list-androidforworkenrollmentprofiles.md)|[androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) collection|Get the androidForWorkEnrollmentProfiles from the androidForWorkEnrollmentProfiles navigation property.|
|[Create androidForWorkEnrollmentProfiles](../api/devicemanagement-post-androidforworkenrollmentprofiles.md)|[androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md)|Create a new androidForWorkEnrollmentProfiles object.|
|[Delete androidForWorkEnrollmentProfiles](../api/devicemanagement-delete-androidforworkenrollmentprofiles.md)|None|Delete an [androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) object.|
|[Update androidForWorkEnrollmentProfiles](../api/devicemanagement-update-androidforworkenrollmentprofiles.md)|[androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md)|Update the properties of an androidForWorkEnrollmentProfiles object.|
|[Get androidForWorkEnrollmentProfile](../api/androidforworkenrollmentprofile-get.md)|[androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md)|Read the properties and relationships of an [androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) object.|
|[List androidManagedStoreAccountEnterpriseSettings](../api/devicemanagement-list-androidmanagedstoreaccountenterprisesettings.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/androidmanagedstoreaccountenterprisesettings.md) collection|Get the androidManagedStoreAccountEnterpriseSettings from the androidManagedStoreAccountEnterpriseSettings navigation property.|
|[Create androidManagedStoreAccountEnterpriseSettings](../api/devicemanagement-post-androidmanagedstoreaccountenterprisesettings.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/androidmanagedstoreaccountenterprisesettings.md)|Create a new androidManagedStoreAccountEnterpriseSettings object.|
|[Delete androidManagedStoreAccountEnterpriseSettings](../api/devicemanagement-delete-androidmanagedstoreaccountenterprisesettings.md)|None|Delete an [androidManagedStoreAccountEnterpriseSettings](../resources/androidmanagedstoreaccountenterprisesettings.md) object.|
|[Update androidManagedStoreAccountEnterpriseSettings](../api/devicemanagement-update-androidmanagedstoreaccountenterprisesettings.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/androidmanagedstoreaccountenterprisesettings.md)|Update the properties of an androidManagedStoreAccountEnterpriseSettings object.|
|[Get androidManagedStoreAccountEnterpriseSettings](../api/androidmanagedstoreaccountenterprisesettings-get.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/androidmanagedstoreaccountenterprisesettings.md)|Read the properties and relationships of an [androidManagedStoreAccountEnterpriseSettings](../resources/androidmanagedstoreaccountenterprisesettings.md) object.|
|[List androidManagedStoreAppConfigurationSchemas](../api/devicemanagement-list-androidmanagedstoreappconfigurationschemas.md)|[androidManagedStoreAppConfigurationSchema](../resources/androidmanagedstoreappconfigurationschema.md) collection|Get the androidManagedStoreAppConfigurationSchemas from the androidManagedStoreAppConfigurationSchemas navigation property.|
|[Create androidManagedStoreAppConfigurationSchemas](../api/devicemanagement-post-androidmanagedstoreappconfigurationschemas.md)|[androidManagedStoreAppConfigurationSchema](../resources/androidmanagedstoreappconfigurationschema.md)|Create a new androidManagedStoreAppConfigurationSchemas object.|
|[Delete androidManagedStoreAppConfigurationSchemas](../api/devicemanagement-delete-androidmanagedstoreappconfigurationschemas.md)|None|Delete an [androidManagedStoreAppConfigurationSchema](../resources/androidmanagedstoreappconfigurationschema.md) object.|
|[Update androidManagedStoreAppConfigurationSchemas](../api/devicemanagement-update-androidmanagedstoreappconfigurationschemas.md)|[androidManagedStoreAppConfigurationSchema](../resources/androidmanagedstoreappconfigurationschema.md)|Update the properties of an androidManagedStoreAppConfigurationSchemas object.|
|[Get androidManagedStoreAppConfigurationSchema](../api/androidmanagedstoreappconfigurationschema-get.md)|[androidManagedStoreAppConfigurationSchema](../resources/androidmanagedstoreappconfigurationschema.md)|Read the properties and relationships of an [androidManagedStoreAppConfigurationSchema](../resources/androidmanagedstoreappconfigurationschema.md) object.|
|[List androidDeviceOwnerEnrollmentProfiles](../api/devicemanagement-list-androiddeviceownerenrollmentprofiles.md)|[androidDeviceOwnerEnrollmentProfile](../resources/androiddeviceownerenrollmentprofile.md) collection|Get the androidDeviceOwnerEnrollmentProfiles from the androidDeviceOwnerEnrollmentProfiles navigation property.|
|[Create androidDeviceOwnerEnrollmentProfiles](../api/devicemanagement-post-androiddeviceownerenrollmentprofiles.md)|[androidDeviceOwnerEnrollmentProfile](../resources/androiddeviceownerenrollmentprofile.md)|Create a new androidDeviceOwnerEnrollmentProfiles object.|
|[Delete androidDeviceOwnerEnrollmentProfiles](../api/devicemanagement-delete-androiddeviceownerenrollmentprofiles.md)|None|Delete an [androidDeviceOwnerEnrollmentProfile](../resources/androiddeviceownerenrollmentprofile.md) object.|
|[Update androidDeviceOwnerEnrollmentProfiles](../api/devicemanagement-update-androiddeviceownerenrollmentprofiles.md)|[androidDeviceOwnerEnrollmentProfile](../resources/androiddeviceownerenrollmentprofile.md)|Update the properties of an androidDeviceOwnerEnrollmentProfiles object.|
|[Get androidDeviceOwnerEnrollmentProfile](../api/androiddeviceownerenrollmentprofile-get.md)|[androidDeviceOwnerEnrollmentProfile](../resources/androiddeviceownerenrollmentprofile.md)|Read the properties and relationships of an [androidDeviceOwnerEnrollmentProfile](../resources/androiddeviceownerenrollmentprofile.md) object.|
|[List termsAndConditions](../api/devicemanagement-list-termsandconditions.md)|[termsAndConditions](../resources/termsandconditions.md) collection|Get the termsAndConditions from the termsAndConditions navigation property.|
|[Create termsAndConditions](../api/devicemanagement-post-termsandconditions.md)|[termsAndConditions](../resources/termsandconditions.md)|Create a new termsAndConditions object.|
|[Delete termsAndConditions](../api/devicemanagement-delete-termsandconditions.md)|None|Delete a [termsAndConditions](../resources/termsandconditions.md) object.|
|[Update termsAndConditions](../api/devicemanagement-update-termsandconditions.md)|[termsAndConditions](../resources/termsandconditions.md)|Update the properties of a termsAndConditions object.|
|[Get termsAndConditions](../api/termsandconditions-get.md)|[termsAndConditions](../resources/termsandconditions.md)|Read the properties and relationships of a [termsAndConditions](../resources/termsandconditions.md) object.|
|[List deviceConfigurations](../api/devicemanagement-list-deviceconfigurations.md)|[deviceConfiguration](../resources/deviceconfiguration.md) collection|Get the deviceConfigurations from the deviceConfigurations navigation property.|
|[Create deviceConfigurations](../api/devicemanagement-post-deviceconfigurations.md)|[deviceConfiguration](../resources/deviceconfiguration.md)|Create a new deviceConfigurations object.|
|[Delete deviceConfigurations](../api/devicemanagement-delete-deviceconfigurations.md)|None|Delete a [deviceConfiguration](../resources/deviceconfiguration.md) object.|
|[Update deviceConfigurations](../api/devicemanagement-update-deviceconfigurations.md)|[deviceConfiguration](../resources/deviceconfiguration.md)|Update the properties of a deviceConfigurations object.|
|[Get deviceConfiguration](../api/deviceconfiguration-get.md)|[deviceConfiguration](../resources/deviceconfiguration.md)|Read the properties and relationships of a [deviceConfiguration](../resources/deviceconfiguration.md) object.|
|[List deviceCompliancePolicies](../api/devicemanagement-list-devicecompliancepolicies.md)|[deviceCompliancePolicy](../resources/devicecompliancepolicy.md) collection|Get the deviceCompliancePolicies from the deviceCompliancePolicies navigation property.|
|[Create deviceCompliancePolicies](../api/devicemanagement-post-devicecompliancepolicies.md)|[deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|Create a new deviceCompliancePolicies object.|
|[Delete deviceCompliancePolicies](../api/devicemanagement-delete-devicecompliancepolicies.md)|None|Delete a [deviceCompliancePolicy](../resources/devicecompliancepolicy.md) object.|
|[Update deviceCompliancePolicies](../api/devicemanagement-update-devicecompliancepolicies.md)|[deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|Update the properties of a deviceCompliancePolicies object.|
|[Get deviceCompliancePolicy](../api/devicecompliancepolicy-get.md)|[deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|Read the properties and relationships of a [deviceCompliancePolicy](../resources/devicecompliancepolicy.md) object.|
|[List softwareUpdateStatusSummary](../api/devicemanagement-list-softwareupdatestatussummary.md)|[softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md) collection|Get the softwareUpdateStatusSummaries from the softwareUpdateStatusSummary navigation property.|
|[Add softwareUpdateStatusSummary](../api/devicemanagement-post-softwareupdatestatussummary.md)|[softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md)|Add softwareUpdateStatusSummary by posting to the softwareUpdateStatusSummary collection.|
|[Remove softwareUpdateStatusSummary](../api/devicemanagement-delete-softwareupdatestatussummary.md)|None|Remove a [softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md) object.|
|[List deviceCompliancePolicyDeviceStateSummary](../api/devicemanagement-list-devicecompliancepolicydevicestatesummary.md)|[deviceCompliancePolicyDeviceStateSummary](../resources/devicecompliancepolicydevicestatesummary.md) collection|Get the deviceCompliancePolicyDeviceStateSummaries from the deviceCompliancePolicyDeviceStateSummary navigation property.|
|[Create deviceCompliancePolicyDeviceStateSummary](../api/devicemanagement-post-devicecompliancepolicydevicestatesummary.md)|[deviceCompliancePolicyDeviceStateSummary](../resources/devicecompliancepolicydevicestatesummary.md)|Create a new deviceCompliancePolicyDeviceStateSummary object.|
|[Delete deviceCompliancePolicyDeviceStateSummary](../api/devicemanagement-delete-devicecompliancepolicydevicestatesummary.md)|None|Delete a [deviceCompliancePolicyDeviceStateSummary](../resources/devicecompliancepolicydevicestatesummary.md) object.|
|[Update deviceCompliancePolicyDeviceStateSummary](../api/devicemanagement-update-devicecompliancepolicydevicestatesummary.md)|[deviceCompliancePolicyDeviceStateSummary](../resources/devicecompliancepolicydevicestatesummary.md)|Update the properties of a deviceCompliancePolicyDeviceStateSummary object.|
|[Get deviceCompliancePolicyDeviceStateSummary](../api/devicecompliancepolicydevicestatesummary-get.md)|[deviceCompliancePolicyDeviceStateSummary](../resources/devicecompliancepolicydevicestatesummary.md)|Read the properties and relationships of a [deviceCompliancePolicyDeviceStateSummary](../resources/devicecompliancepolicydevicestatesummary.md) object.|
|[List deviceCompliancePolicySettingStateSummaries](../api/devicemanagement-list-devicecompliancepolicysettingstatesummaries.md)|[deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md) collection|Get the deviceCompliancePolicySettingStateSummaries from the deviceCompliancePolicySettingStateSummaries navigation property.|
|[Create deviceCompliancePolicySettingStateSummaries](../api/devicemanagement-post-devicecompliancepolicysettingstatesummaries.md)|[deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md)|Create a new deviceCompliancePolicySettingStateSummaries object.|
|[Delete deviceCompliancePolicySettingStateSummaries](../api/devicemanagement-delete-devicecompliancepolicysettingstatesummaries.md)|None|Delete a [deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md) object.|
|[Update deviceCompliancePolicySettingStateSummaries](../api/devicemanagement-update-devicecompliancepolicysettingstatesummaries.md)|[deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md)|Update the properties of a deviceCompliancePolicySettingStateSummaries object.|
|[Get deviceCompliancePolicySettingStateSummary](../api/devicecompliancepolicysettingstatesummary-get.md)|[deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md)|Read the properties and relationships of a [deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md) object.|
|[List advancedThreatProtectionOnboardingStateSummary](../api/devicemanagement-list-advancedthreatprotectiononboardingstatesummary.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md) collection|Get the advancedThreatProtectionOnboardingStateSummaries from the advancedThreatProtectionOnboardingStateSummary navigation property.|
|[Create advancedThreatProtectionOnboardingStateSummary](../api/devicemanagement-post-advancedthreatprotectiononboardingstatesummary.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md)|Create a new advancedThreatProtectionOnboardingStateSummary object.|
|[Delete advancedThreatProtectionOnboardingStateSummary](../api/devicemanagement-delete-advancedthreatprotectiononboardingstatesummary.md)|None|Delete an [advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md) object.|
|[Update advancedThreatProtectionOnboardingStateSummary](../api/devicemanagement-update-advancedthreatprotectiononboardingstatesummary.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md)|Update the properties of an advancedThreatProtectionOnboardingStateSummary object.|
|[Get advancedThreatProtectionOnboardingStateSummary](../api/advancedthreatprotectiononboardingstatesummary-get.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md)|Read the properties and relationships of an [advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md) object.|
|[List deviceConfigurationDeviceStateSummaries](../api/devicemanagement-list-deviceconfigurationdevicestatesummaries.md)|[deviceConfigurationDeviceStateSummary](../resources/deviceconfigurationdevicestatesummary.md) collection|Get the deviceConfigurationDeviceStateSummaries from the deviceConfigurationDeviceStateSummaries navigation property.|
|[Create deviceConfigurationDeviceStateSummaries](../api/devicemanagement-post-deviceconfigurationdevicestatesummaries.md)|[deviceConfigurationDeviceStateSummary](../resources/deviceconfigurationdevicestatesummary.md)|Create a new deviceConfigurationDeviceStateSummaries object.|
|[Delete deviceConfigurationDeviceStateSummaries](../api/devicemanagement-delete-deviceconfigurationdevicestatesummaries.md)|None|Delete a [deviceConfigurationDeviceStateSummary](../resources/deviceconfigurationdevicestatesummary.md) object.|
|[Update deviceConfigurationDeviceStateSummaries](../api/devicemanagement-update-deviceconfigurationdevicestatesummaries.md)|[deviceConfigurationDeviceStateSummary](../resources/deviceconfigurationdevicestatesummary.md)|Update the properties of a deviceConfigurationDeviceStateSummaries object.|
|[Get deviceConfigurationDeviceStateSummary](../api/deviceconfigurationdevicestatesummary-get.md)|[deviceConfigurationDeviceStateSummary](../resources/deviceconfigurationdevicestatesummary.md)|Read the properties and relationships of a [deviceConfigurationDeviceStateSummary](../resources/deviceconfigurationdevicestatesummary.md) object.|
|[List deviceConfigurationUserStateSummaries](../api/devicemanagement-list-deviceconfigurationuserstatesummaries.md)|[deviceConfigurationUserStateSummary](../resources/deviceconfigurationuserstatesummary.md) collection|Get the deviceConfigurationUserStateSummaries from the deviceConfigurationUserStateSummaries navigation property.|
|[Create deviceConfigurationUserStateSummaries](../api/devicemanagement-post-deviceconfigurationuserstatesummaries.md)|[deviceConfigurationUserStateSummary](../resources/deviceconfigurationuserstatesummary.md)|Create a new deviceConfigurationUserStateSummaries object.|
|[Delete deviceConfigurationUserStateSummaries](../api/devicemanagement-delete-deviceconfigurationuserstatesummaries.md)|None|Delete a [deviceConfigurationUserStateSummary](../resources/deviceconfigurationuserstatesummary.md) object.|
|[Update deviceConfigurationUserStateSummaries](../api/devicemanagement-update-deviceconfigurationuserstatesummaries.md)|[deviceConfigurationUserStateSummary](../resources/deviceconfigurationuserstatesummary.md)|Update the properties of a deviceConfigurationUserStateSummaries object.|
|[Get deviceConfigurationUserStateSummary](../api/deviceconfigurationuserstatesummary-get.md)|[deviceConfigurationUserStateSummary](../resources/deviceconfigurationuserstatesummary.md)|Read the properties and relationships of a [deviceConfigurationUserStateSummary](../resources/deviceconfigurationuserstatesummary.md) object.|
|[List cartToClassAssociations](../api/devicemanagement-list-carttoclassassociations.md)|[cartToClassAssociation](../resources/carttoclassassociation.md) collection|Get the cartToClassAssociations from the cartToClassAssociations navigation property.|
|[Create cartToClassAssociations](../api/devicemanagement-post-carttoclassassociations.md)|[cartToClassAssociation](../resources/carttoclassassociation.md)|Create a new cartToClassAssociations object.|
|[Delete cartToClassAssociations](../api/devicemanagement-delete-carttoclassassociations.md)|None|Delete a [cartToClassAssociation](../resources/carttoclassassociation.md) object.|
|[Update cartToClassAssociations](../api/devicemanagement-update-carttoclassassociations.md)|[cartToClassAssociation](../resources/carttoclassassociation.md)|Update the properties of a cartToClassAssociations object.|
|[Get cartToClassAssociation](../api/carttoclassassociation-get.md)|[cartToClassAssociation](../resources/carttoclassassociation.md)|Read the properties and relationships of a [cartToClassAssociation](../resources/carttoclassassociation.md) object.|
|[List iosUpdateStatuses](../api/devicemanagement-list-iosupdatestatuses.md)|[iosUpdateDeviceStatus](../resources/iosupdatedevicestatus.md) collection|Get the iosUpdateDeviceStatus from the iosUpdateStatuses navigation property.|
|[Create iosUpdateStatuses](../api/devicemanagement-post-iosupdatestatuses.md)|[iosUpdateDeviceStatus](../resources/iosupdatedevicestatus.md)|Create a new iosUpdateStatuses object.|
|[Delete iosUpdateStatuses](../api/devicemanagement-delete-iosupdatestatuses.md)|None|Delete an [iosUpdateDeviceStatus](../resources/iosupdatedevicestatus.md) object.|
|[Update iosUpdateStatuses](../api/devicemanagement-update-iosupdatestatuses.md)|[iosUpdateDeviceStatus](../resources/iosupdatedevicestatus.md)|Update the properties of an iosUpdateStatuses object.|
|[Get iosUpdateDeviceStatus](../api/iosupdatedevicestatus-get.md)|[iosUpdateDeviceStatus](../resources/iosupdatedevicestatus.md)|Read the properties and relationships of an [iosUpdateDeviceStatus](../resources/iosupdatedevicestatus.md) object.|
|[List ndesConnectors](../api/devicemanagement-list-ndesconnectors.md)|[ndesConnector](../resources/ndesconnector.md) collection|Get the ndesConnectors from the ndesConnectors navigation property.|
|[Create ndesConnectors](../api/devicemanagement-post-ndesconnectors.md)|[ndesConnector](../resources/ndesconnector.md)|Create a new ndesConnectors object.|
|[Delete ndesConnectors](../api/devicemanagement-delete-ndesconnectors.md)|None|Delete a [ndesConnector](../resources/ndesconnector.md) object.|
|[Update ndesConnectors](../api/devicemanagement-update-ndesconnectors.md)|[ndesConnector](../resources/ndesconnector.md)|Update the properties of a ndesConnectors object.|
|[Get ndesConnector](../api/ndesconnector-get.md)|[ndesConnector](../resources/ndesconnector.md)|Read the properties and relationships of a [ndesConnector](../resources/ndesconnector.md) object.|
|[List deviceConfigurationRestrictedAppsViolations](../api/devicemanagement-list-deviceconfigurationrestrictedappsviolations.md)|[restrictedAppsViolation](../resources/restrictedappsviolation.md) collection|Get the restrictedAppsViolations from the deviceConfigurationRestrictedAppsViolations navigation property.|
|[Create deviceConfigurationRestrictedAppsViolations](../api/devicemanagement-post-deviceconfigurationrestrictedappsviolations.md)|[restrictedAppsViolation](../resources/restrictedappsviolation.md)|Create a new deviceConfigurationRestrictedAppsViolations object.|
|[Delete deviceConfigurationRestrictedAppsViolations](../api/devicemanagement-delete-deviceconfigurationrestrictedappsviolations.md)|None|Delete a [restrictedAppsViolation](../resources/restrictedappsviolation.md) object.|
|[Update deviceConfigurationRestrictedAppsViolations](../api/devicemanagement-update-deviceconfigurationrestrictedappsviolations.md)|[restrictedAppsViolation](../resources/restrictedappsviolation.md)|Update the properties of a deviceConfigurationRestrictedAppsViolations object.|
|[Get restrictedAppsViolation](../api/restrictedappsviolation-get.md)|[restrictedAppsViolation](../resources/restrictedappsviolation.md)|Read the properties and relationships of a [restrictedAppsViolation](../resources/restrictedappsviolation.md) object.|
|[List managedDeviceEncryptionStates](../api/devicemanagement-list-manageddeviceencryptionstates.md)|[managedDeviceEncryptionState](../resources/manageddeviceencryptionstate.md) collection|Get the managedDeviceEncryptionStates from the managedDeviceEncryptionStates navigation property.|
|[Create managedDeviceEncryptionStates](../api/devicemanagement-post-manageddeviceencryptionstates.md)|[managedDeviceEncryptionState](../resources/manageddeviceencryptionstate.md)|Create a new managedDeviceEncryptionStates object.|
|[Delete managedDeviceEncryptionStates](../api/devicemanagement-delete-manageddeviceencryptionstates.md)|None|Delete a [managedDeviceEncryptionState](../resources/manageddeviceencryptionstate.md) object.|
|[Update managedDeviceEncryptionStates](../api/devicemanagement-update-manageddeviceencryptionstates.md)|[managedDeviceEncryptionState](../resources/manageddeviceencryptionstate.md)|Update the properties of a managedDeviceEncryptionStates object.|
|[Get managedDeviceEncryptionState](../api/manageddeviceencryptionstate-get.md)|[managedDeviceEncryptionState](../resources/manageddeviceencryptionstate.md)|Read the properties and relationships of a [managedDeviceEncryptionState](../resources/manageddeviceencryptionstate.md) object.|
|[List deviceConfigurationConflictSummary](../api/devicemanagement-list-deviceconfigurationconflictsummary.md)|[deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md) collection|Get the deviceConfigurationConflictSummaries from the deviceConfigurationConflictSummary navigation property.|
|[Create deviceConfigurationConflictSummary](../api/devicemanagement-post-deviceconfigurationconflictsummary.md)|[deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md)|Create a new deviceConfigurationConflictSummary object.|
|[Delete deviceConfigurationConflictSummary](../api/devicemanagement-delete-deviceconfigurationconflictsummary.md)|None|Delete a [deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md) object.|
|[Update deviceConfigurationConflictSummary](../api/devicemanagement-update-deviceconfigurationconflictsummary.md)|[deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md)|Update the properties of a deviceConfigurationConflictSummary object.|
|[Get deviceConfigurationConflictSummary](../api/deviceconfigurationconflictsummary-get.md)|[deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md)|Read the properties and relationships of a [deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md) object.|
|[List deviceConfigurationsAllManagedDeviceCertificateStates](../api/devicemanagement-list-deviceconfigurationsallmanageddevicecertificatestates.md)|[managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md) collection|Get the managedAllDeviceCertificateStates from the deviceConfigurationsAllManagedDeviceCertificateStates navigation property.|
|[Create deviceConfigurationsAllManagedDeviceCertificateStates](../api/devicemanagement-post-deviceconfigurationsallmanageddevicecertificatestates.md)|[managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md)|Create a new deviceConfigurationsAllManagedDeviceCertificateStates object.|
|[Delete deviceConfigurationsAllManagedDeviceCertificateStates](../api/devicemanagement-delete-deviceconfigurationsallmanageddevicecertificatestates.md)|None|Delete a [managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md) object.|
|[Update deviceConfigurationsAllManagedDeviceCertificateStates](../api/devicemanagement-update-deviceconfigurationsallmanageddevicecertificatestates.md)|[managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md)|Update the properties of a deviceConfigurationsAllManagedDeviceCertificateStates object.|
|[Get managedAllDeviceCertificateState](../api/managedalldevicecertificatestate-get.md)|[managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md)|Read the properties and relationships of a [managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md) object.|
|[List deviceCategories](../api/devicemanagement-list-devicecategories.md)|[deviceCategory](../resources/devicecategory.md) collection|Get the deviceCategories from the deviceCategories navigation property.|
|[Create deviceCategories](../api/devicemanagement-post-devicecategories.md)|[deviceCategory](../resources/devicecategory.md)|Create a new deviceCategories object.|
|[Delete deviceCategories](../api/devicemanagement-delete-devicecategories.md)|None|Delete a [deviceCategory](../resources/devicecategory.md) object.|
|[Update deviceCategories](../api/devicemanagement-update-devicecategories.md)|[deviceCategory](../resources/devicecategory.md)|Update the properties of a deviceCategories object.|
|[Get deviceCategory](../api/devicecategory-get.md)|[deviceCategory](../resources/devicecategory.md)|Read the properties and relationships of a [deviceCategory](../resources/devicecategory.md) object.|
|[List exchangeConnectors](../api/devicemanagement-list-exchangeconnectors.md)|[deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) collection|Get the deviceManagementExchangeConnectors from the exchangeConnectors navigation property.|
|[Create exchangeConnectors](../api/devicemanagement-post-exchangeconnectors.md)|[deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md)|Create a new exchangeConnectors object.|
|[Delete exchangeConnectors](../api/devicemanagement-delete-exchangeconnectors.md)|None|Delete an [deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) object.|
|[Update exchangeConnectors](../api/devicemanagement-update-exchangeconnectors.md)|[deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md)|Update the properties of an exchangeConnectors object.|
|[Get deviceManagementExchangeConnector](../api/devicemanagementexchangeconnector-get.md)|[deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md)|Read the properties and relationships of a [deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) object.|
|[List deviceEnrollmentConfigurations](../api/devicemanagement-list-deviceenrollmentconfigurations.md)|[deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md) collection|Get the deviceEnrollmentConfigurations from the deviceEnrollmentConfigurations navigation property.|
|[Create deviceEnrollmentConfigurations](../api/devicemanagement-post-deviceenrollmentconfigurations.md)|[deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|Create a new deviceEnrollmentConfigurations object.|
|[Delete deviceEnrollmentConfigurations](../api/devicemanagement-delete-deviceenrollmentconfigurations.md)|None|Delete a [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md) object.|
|[Update deviceEnrollmentConfigurations](../api/devicemanagement-update-deviceenrollmentconfigurations.md)|[deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|Update the properties of a deviceEnrollmentConfigurations object.|
|[Get deviceEnrollmentConfiguration](../api/deviceenrollmentconfiguration-get.md)|[deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|Read the properties and relationships of a [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md) object.|
|[List exchangeOnPremisesPolicy](../api/devicemanagement-list-exchangeonpremisespolicy.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md) collection|Get the deviceManagementExchangeOnPremisesPolicies from the exchangeOnPremisesPolicy navigation property.|
|[Create exchangeOnPremisesPolicy](../api/devicemanagement-post-exchangeonpremisespolicy.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md)|Create a new exchangeOnPremisesPolicy object.|
|[Delete exchangeOnPremisesPolicy](../api/devicemanagement-delete-exchangeonpremisespolicy.md)|None|Delete an [deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md) object.|
|[Update exchangeOnPremisesPolicy](../api/devicemanagement-update-exchangeonpremisespolicy.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md)|Update the properties of an exchangeOnPremisesPolicy object.|
|[Get deviceManagementExchangeOnPremisesPolicy](../api/devicemanagementexchangeonpremisespolicy-get.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md)|Read the properties and relationships of a [deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md) object.|
|[List exchangeOnPremisesPolicies](../api/devicemanagement-list-exchangeonpremisespolicies.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md) collection|Get the deviceManagementExchangeOnPremisesPolicies from the exchangeOnPremisesPolicies navigation property.|
|[Create exchangeOnPremisesPolicies](../api/devicemanagement-post-exchangeonpremisespolicies.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md)|Create a new exchangeOnPremisesPolicies object.|
|[Delete exchangeOnPremisesPolicies](../api/devicemanagement-delete-exchangeonpremisespolicies.md)|None|Delete an [deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md) object.|
|[Update exchangeOnPremisesPolicies](../api/devicemanagement-update-exchangeonpremisespolicies.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md)|Update the properties of an exchangeOnPremisesPolicies object.|
|[Get deviceManagementExchangeOnPremisesPolicy](../api/devicemanagementexchangeonpremisespolicy-get.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md)|Read the properties and relationships of a [deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md) object.|
|[List conditionalAccessSettings](../api/devicemanagement-list-conditionalaccesssettings.md)|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) collection|Get the onPremisesConditionalAccessSettings from the conditionalAccessSettings navigation property.|
|[Create conditionalAccessSettings](../api/devicemanagement-post-conditionalaccesssettings.md)|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md)|Create a new conditionalAccessSettings object.|
|[Delete conditionalAccessSettings](../api/devicemanagement-delete-conditionalaccesssettings.md)|None|Delete a [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.|
|[Update conditionalAccessSettings](../api/devicemanagement-update-conditionalaccesssettings.md)|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md)|Update the properties of a conditionalAccessSettings object.|
|[Get onPremisesConditionalAccessSettings](../api/onpremisesconditionalaccesssettings-get.md)|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md)|Read the properties and relationships of an [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.|
|[List mobileThreatDefenseConnectors](../api/devicemanagement-list-mobilethreatdefenseconnectors.md)|[mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) collection|Get the mobileThreatDefenseConnectors from the mobileThreatDefenseConnectors navigation property.|
|[Create mobileThreatDefenseConnectors](../api/devicemanagement-post-mobilethreatdefenseconnectors.md)|[mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md)|Create a new mobileThreatDefenseConnectors object.|
|[Delete mobileThreatDefenseConnectors](../api/devicemanagement-delete-mobilethreatdefenseconnectors.md)|None|Delete a [mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) object.|
|[Update mobileThreatDefenseConnectors](../api/devicemanagement-update-mobilethreatdefenseconnectors.md)|[mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md)|Update the properties of a mobileThreatDefenseConnectors object.|
|[Get mobileThreatDefenseConnector](../api/mobilethreatdefenseconnector-get.md)|[mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md)|Read the properties and relationships of a [mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) object.|
|[List deviceManagementPartners](../api/devicemanagement-list-devicemanagementpartners.md)|[deviceManagementPartner](../resources/devicemanagementpartner.md) collection|Get the deviceManagementPartners from the deviceManagementPartners navigation property.|
|[Create deviceManagementPartners](../api/devicemanagement-post-devicemanagementpartners.md)|[deviceManagementPartner](../resources/devicemanagementpartner.md)|Create a new deviceManagementPartners object.|
|[Delete deviceManagementPartners](../api/devicemanagement-delete-devicemanagementpartners.md)|None|Delete a [deviceManagementPartner](../resources/devicemanagementpartner.md) object.|
|[Update deviceManagementPartners](../api/devicemanagement-update-devicemanagementpartners.md)|[deviceManagementPartner](../resources/devicemanagementpartner.md)|Update the properties of a deviceManagementPartners object.|
|[Get deviceManagementPartner](../api/devicemanagementpartner-get.md)|[deviceManagementPartner](../resources/devicemanagementpartner.md)|Read the properties and relationships of a [deviceManagementPartner](../resources/devicemanagementpartner.md) object.|
|[List complianceManagementPartners](../api/devicemanagement-list-compliancemanagementpartners.md)|[complianceManagementPartner](../resources/compliancemanagementpartner.md) collection|Get the complianceManagementPartners from the complianceManagementPartners navigation property.|
|[Create complianceManagementPartners](../api/devicemanagement-post-compliancemanagementpartners.md)|[complianceManagementPartner](../resources/compliancemanagementpartner.md)|Create a new complianceManagementPartners object.|
|[Delete complianceManagementPartners](../api/devicemanagement-delete-compliancemanagementpartners.md)|None|Delete a [complianceManagementPartner](../resources/compliancemanagementpartner.md) object.|
|[Update complianceManagementPartners](../api/devicemanagement-update-compliancemanagementpartners.md)|[complianceManagementPartner](../resources/compliancemanagementpartner.md)|Update the properties of a complianceManagementPartners object.|
|[Get complianceManagementPartner](../api/compliancemanagementpartner-get.md)|[complianceManagementPartner](../resources/compliancemanagementpartner.md)|Read the properties and relationships of a [complianceManagementPartner](../resources/compliancemanagementpartner.md) object.|
|[List intents](../api/devicemanagement-list-intents.md)|[deviceManagementIntent](../resources/devicemanagementintent.md) collection|Get the deviceManagementIntents from the intents navigation property.|
|[Create intents](../api/devicemanagement-post-intents.md)|[deviceManagementIntent](../resources/devicemanagementintent.md)|Create a new intents object.|
|[Delete intents](../api/devicemanagement-delete-intents.md)|None|Delete an [deviceManagementIntent](../resources/devicemanagementintent.md) object.|
|[Update intents](../api/devicemanagement-update-intents.md)|[deviceManagementIntent](../resources/devicemanagementintent.md)|Update the properties of an intents object.|
|[Get deviceManagementIntent](../api/devicemanagementintent-get.md)|[deviceManagementIntent](../resources/devicemanagementintent.md)|Read the properties and relationships of a [deviceManagementIntent](../resources/devicemanagementintent.md) object.|
|[List settingDefinitions](../api/devicemanagement-list-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) collection|Get the deviceManagementSettingDefinitions from the settingDefinitions navigation property.|
|[Create settingDefinitions](../api/devicemanagement-post-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|Create a new settingDefinitions object.|
|[Delete settingDefinitions](../api/devicemanagement-delete-settingdefinitions.md)|None|Delete a [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) object.|
|[Update settingDefinitions](../api/devicemanagement-update-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|Update the properties of a settingDefinitions object.|
|[Get deviceManagementSettingDefinition](../api/devicemanagementsettingdefinition-get.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|Read the properties and relationships of a [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) object.|
|[List templates](../api/devicemanagement-list-templates.md)|[deviceManagementTemplate](../resources/devicemanagementtemplate.md) collection|Get the deviceManagementTemplates from the templates navigation property.|
|[Create templates](../api/devicemanagement-post-templates.md)|[deviceManagementTemplate](../resources/devicemanagementtemplate.md)|Create a new templates object.|
|[Delete templates](../api/devicemanagement-delete-templates.md)|None|Delete a [deviceManagementTemplate](../resources/devicemanagementtemplate.md) object.|
|[Update templates](../api/devicemanagement-update-templates.md)|[deviceManagementTemplate](../resources/devicemanagementtemplate.md)|Update the properties of a templates object.|
|[Get deviceManagementTemplate](../api/devicemanagementtemplate-get.md)|[deviceManagementTemplate](../resources/devicemanagementtemplate.md)|Read the properties and relationships of a [deviceManagementTemplate](../resources/devicemanagementtemplate.md) object.|
|[List categories](../api/devicemanagement-list-categories.md)|[deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) collection|Get the deviceManagementSettingCategories from the categories navigation property.|
|[Create categories](../api/devicemanagement-post-categories.md)|[deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|Create a new categories object.|
|[Delete categories](../api/devicemanagement-delete-categories.md)|None|Delete a [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) object.|
|[Update categories](../api/devicemanagement-update-categories.md)|[deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|Update the properties of a categories object.|
|[Get deviceManagementSettingCategory](../api/devicemanagementsettingcategory-get.md)|[deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|Read the properties and relationships of a [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) object.|
|[List remoteActionAudits](../api/devicemanagement-list-remoteactionaudits.md)|[remoteActionAudit](../resources/remoteactionaudit.md) collection|Get the remoteActionAudits from the remoteActionAudits navigation property.|
|[Create remoteActionAudits](../api/devicemanagement-post-remoteactionaudits.md)|[remoteActionAudit](../resources/remoteactionaudit.md)|Create a new remoteActionAudits object.|
|[Delete remoteActionAudits](../api/devicemanagement-delete-remoteactionaudits.md)|None|Delete a [remoteActionAudit](../resources/remoteactionaudit.md) object.|
|[Update remoteActionAudits](../api/devicemanagement-update-remoteactionaudits.md)|[remoteActionAudit](../resources/remoteactionaudit.md)|Update the properties of a remoteActionAudits object.|
|[Get remoteActionAudit](../api/remoteactionaudit-get.md)|[remoteActionAudit](../resources/remoteactionaudit.md)|Read the properties and relationships of a [remoteActionAudit](../resources/remoteactionaudit.md) object.|
|[List applePushNotificationCertificate](../api/devicemanagement-list-applepushnotificationcertificate.md)|[applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) collection|Get the applePushNotificationCertificates from the applePushNotificationCertificate navigation property.|
|[Create applePushNotificationCertificate](../api/devicemanagement-post-applepushnotificationcertificate.md)|[applePushNotificationCertificate](../resources/applepushnotificationcertificate.md)|Create a new applePushNotificationCertificate object.|
|[Delete applePushNotificationCertificate](../api/devicemanagement-delete-applepushnotificationcertificate.md)|None|Delete an [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object.|
|[Update applePushNotificationCertificate](../api/devicemanagement-update-applepushnotificationcertificate.md)|[applePushNotificationCertificate](../resources/applepushnotificationcertificate.md)|Update the properties of an applePushNotificationCertificate object.|
|[Get applePushNotificationCertificate](../api/applepushnotificationcertificate-get.md)|[applePushNotificationCertificate](../resources/applepushnotificationcertificate.md)|Read the properties and relationships of an [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object.|
|[List deviceManagementScripts](../api/devicemanagement-list-devicemanagementscripts.md)|[deviceManagementScript](../resources/devicemanagementscript.md) collection|Get the deviceManagementScripts from the deviceManagementScripts navigation property.|
|[Create deviceManagementScripts](../api/devicemanagement-post-devicemanagementscripts.md)|[deviceManagementScript](../resources/devicemanagementscript.md)|Create a new deviceManagementScripts object.|
|[Delete deviceManagementScripts](../api/devicemanagement-delete-devicemanagementscripts.md)|None|Delete a [deviceManagementScript](../resources/devicemanagementscript.md) object.|
|[Update deviceManagementScripts](../api/devicemanagement-update-devicemanagementscripts.md)|[deviceManagementScript](../resources/devicemanagementscript.md)|Update the properties of a deviceManagementScripts object.|
|[Get deviceManagementScript](../api/devicemanagementscript-get.md)|[deviceManagementScript](../resources/devicemanagementscript.md)|Read the properties and relationships of a [deviceManagementScript](../resources/devicemanagementscript.md) object.|
|[List deviceShellScripts](../api/devicemanagement-list-deviceshellscripts.md)|[deviceShellScript](../resources/deviceshellscript.md) collection|Get the deviceShellScripts from the deviceShellScripts navigation property.|
|[Create deviceShellScripts](../api/devicemanagement-post-deviceshellscripts.md)|[deviceShellScript](../resources/deviceshellscript.md)|Create a new deviceShellScripts object.|
|[Delete deviceShellScripts](../api/devicemanagement-delete-deviceshellscripts.md)|None|Delete a [deviceShellScript](../resources/deviceshellscript.md) object.|
|[Update deviceShellScripts](../api/devicemanagement-update-deviceshellscripts.md)|[deviceShellScript](../resources/deviceshellscript.md)|Update the properties of a deviceShellScripts object.|
|[Get deviceShellScript](../api/deviceshellscript-get.md)|[deviceShellScript](../resources/deviceshellscript.md)|Read the properties and relationships of a [deviceShellScript](../resources/deviceshellscript.md) object.|
|[List deviceHealthScripts](../api/devicemanagement-list-devicehealthscripts.md)|[deviceHealthScript](../resources/devicehealthscript.md) collection|Get the deviceHealthScripts from the deviceHealthScripts navigation property.|
|[Create deviceHealthScripts](../api/devicemanagement-post-devicehealthscripts.md)|[deviceHealthScript](../resources/devicehealthscript.md)|Create a new deviceHealthScripts object.|
|[Delete deviceHealthScripts](../api/devicemanagement-delete-devicehealthscripts.md)|None|Delete a [deviceHealthScript](../resources/devicehealthscript.md) object.|
|[Update deviceHealthScripts](../api/devicemanagement-update-devicehealthscripts.md)|[deviceHealthScript](../resources/devicehealthscript.md)|Update the properties of a deviceHealthScripts object.|
|[Get deviceHealthScript](../api/devicehealthscript-get.md)|[deviceHealthScript](../resources/devicehealthscript.md)|Read the properties and relationships of a [deviceHealthScript](../resources/devicehealthscript.md) object.|
|[List managedDeviceOverview](../api/devicemanagement-list-manageddeviceoverview.md)|[managedDeviceOverview](../resources/manageddeviceoverview.md) collection|Get the managedDeviceOverviews from the managedDeviceOverview navigation property.|
|[Add managedDeviceOverview](../api/devicemanagement-post-manageddeviceoverview.md)|[managedDeviceOverview](../resources/manageddeviceoverview.md)|Add managedDeviceOverview by posting to the managedDeviceOverview collection.|
|[Remove managedDeviceOverview](../api/devicemanagement-delete-manageddeviceoverview.md)|None|Remove a [managedDeviceOverview](../resources/manageddeviceoverview.md) object.|
|[List detectedApps](../api/devicemanagement-list-detectedapps.md)|[detectedApp](../resources/detectedapp.md) collection|Get the detectedApps from the detectedApps navigation property.|
|[Create detectedApps](../api/devicemanagement-post-detectedapps.md)|[detectedApp](../resources/detectedapp.md)|Create a new detectedApps object.|
|[Delete detectedApps](../api/devicemanagement-delete-detectedapps.md)|None|Delete a [detectedApp](../resources/detectedapp.md) object.|
|[Update detectedApps](../api/devicemanagement-update-detectedapps.md)|[detectedApp](../resources/detectedapp.md)|Update the properties of a detectedApps object.|
|[Get detectedApp](../api/detectedapp-get.md)|[detectedApp](../resources/detectedapp.md)|Read the properties and relationships of a [detectedApp](../resources/detectedapp.md) object.|
|[List managedDevices](../api/devicemanagement-list-manageddevices.md)|[managedDevice](../resources/manageddevice.md) collection|Get the managedDevices from the managedDevices navigation property.|
|[Create managedDevices](../api/devicemanagement-post-manageddevices.md)|[managedDevice](../resources/manageddevice.md)|Create a new managedDevices object.|
|[Delete managedDevices](../api/devicemanagement-delete-manageddevices.md)|None|Delete a [managedDevice](../resources/manageddevice.md) object.|
|[Update managedDevices](../api/devicemanagement-update-manageddevices.md)|[managedDevice](../resources/manageddevice.md)|Update the properties of a managedDevices object.|
|[Get managedDevice](../api/manageddevice-get.md)|[managedDevice](../resources/manageddevice.md)|Read the properties and relationships of a [managedDevice](../resources/manageddevice.md) object.|
|[List windowsMalwareInformation](../api/devicemanagement-list-windowsmalwareinformation.md)|[windowsMalwareInformation](../resources/windowsmalwareinformation.md) collection|Get the windowsMalwareInformations from the windowsMalwareInformation navigation property.|
|[Create windowsMalwareInformation](../api/devicemanagement-post-windowsmalwareinformation.md)|[windowsMalwareInformation](../resources/windowsmalwareinformation.md)|Create a new windowsMalwareInformation object.|
|[Delete windowsMalwareInformation](../api/devicemanagement-delete-windowsmalwareinformation.md)|None|Delete a [windowsMalwareInformation](../resources/windowsmalwareinformation.md) object.|
|[Update windowsMalwareInformation](../api/devicemanagement-update-windowsmalwareinformation.md)|[windowsMalwareInformation](../resources/windowsmalwareinformation.md)|Update the properties of a windowsMalwareInformation object.|
|[Get windowsMalwareInformation](../api/windowsmalwareinformation-get.md)|[windowsMalwareInformation](../resources/windowsmalwareinformation.md)|Read the properties and relationships of a [windowsMalwareInformation](../resources/windowsmalwareinformation.md) object.|
|[List dataSharingConsents](../api/devicemanagement-list-datasharingconsents.md)|[dataSharingConsent](../resources/datasharingconsent.md) collection|Get the dataSharingConsents from the dataSharingConsents navigation property.|
|[Create dataSharingConsents](../api/devicemanagement-post-datasharingconsents.md)|[dataSharingConsent](../resources/datasharingconsent.md)|Create a new dataSharingConsents object.|
|[Delete dataSharingConsents](../api/devicemanagement-delete-datasharingconsents.md)|None|Delete a [dataSharingConsent](../resources/datasharingconsent.md) object.|
|[Update dataSharingConsents](../api/devicemanagement-update-datasharingconsents.md)|[dataSharingConsent](../resources/datasharingconsent.md)|Update the properties of a dataSharingConsents object.|
|[Get dataSharingConsent](../api/datasharingconsent-get.md)|[dataSharingConsent](../resources/datasharingconsent.md)|Read the properties and relationships of a [dataSharingConsent](../resources/datasharingconsent.md) object.|
|[List mobileAppTroubleshootingEvents](../api/devicemanagement-list-mobileapptroubleshootingevents.md)|[mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md) collection|Get the mobileAppTroubleshootingEvents from the mobileAppTroubleshootingEvents navigation property.|
|[Create mobileAppTroubleshootingEvents](../api/devicemanagement-post-mobileapptroubleshootingevents.md)|[mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md)|Create a new mobileAppTroubleshootingEvents object.|
|[Delete mobileAppTroubleshootingEvents](../api/devicemanagement-delete-mobileapptroubleshootingevents.md)|None|Delete a [mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md) object.|
|[Update mobileAppTroubleshootingEvents](../api/devicemanagement-update-mobileapptroubleshootingevents.md)|[mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md)|Update the properties of a mobileAppTroubleshootingEvents object.|
|[Get mobileAppTroubleshootingEvent](../api/mobileapptroubleshootingevent-get.md)|[mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md)|Read the properties and relationships of a [mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md) object.|
|[List userExperienceAnalyticsOverview](../api/devicemanagement-list-userexperienceanalyticsoverview.md)|[userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md) collection|Get the userExperienceAnalyticsOverviews from the userExperienceAnalyticsOverview navigation property.|
|[Create userExperienceAnalyticsOverview](../api/devicemanagement-post-userexperienceanalyticsoverview.md)|[userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md)|Create a new userExperienceAnalyticsOverview object.|
|[Delete userExperienceAnalyticsOverview](../api/devicemanagement-delete-userexperienceanalyticsoverview.md)|None|Delete a [userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md) object.|
|[Update userExperienceAnalyticsOverview](../api/devicemanagement-update-userexperienceanalyticsoverview.md)|[userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md)|Update the properties of a userExperienceAnalyticsOverview object.|
|[Get userExperienceAnalyticsOverview](../api/userexperienceanalyticsoverview-get.md)|[userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md)|Read the properties and relationships of a [userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md) object.|
|[List userExperienceAnalyticsBaselines](../api/devicemanagement-list-userexperienceanalyticsbaselines.md)|[userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md) collection|Get the userExperienceAnalyticsBaselines from the userExperienceAnalyticsBaselines navigation property.|
|[Create userExperienceAnalyticsBaselines](../api/devicemanagement-post-userexperienceanalyticsbaselines.md)|[userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md)|Create a new userExperienceAnalyticsBaselines object.|
|[Delete userExperienceAnalyticsBaselines](../api/devicemanagement-delete-userexperienceanalyticsbaselines.md)|None|Delete a [userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md) object.|
|[Update userExperienceAnalyticsBaselines](../api/devicemanagement-update-userexperienceanalyticsbaselines.md)|[userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md)|Update the properties of a userExperienceAnalyticsBaselines object.|
|[Get userExperienceAnalyticsBaseline](../api/userexperienceanalyticsbaseline-get.md)|[userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md)|Read the properties and relationships of a [userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md) object.|
|[List userExperienceAnalyticsCategories](../api/devicemanagement-list-userexperienceanalyticscategories.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) collection|Get the userExperienceAnalyticsCategories from the userExperienceAnalyticsCategories navigation property.|
|[Create userExperienceAnalyticsCategories](../api/devicemanagement-post-userexperienceanalyticscategories.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|Create a new userExperienceAnalyticsCategories object.|
|[Delete userExperienceAnalyticsCategories](../api/devicemanagement-delete-userexperienceanalyticscategories.md)|None|Delete a [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) object.|
|[Update userExperienceAnalyticsCategories](../api/devicemanagement-update-userexperienceanalyticscategories.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|Update the properties of a userExperienceAnalyticsCategories object.|
|[Get userExperienceAnalyticsCategory](../api/userexperienceanalyticscategory-get.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|Read the properties and relationships of a [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) object.|
|[List userExperienceAnalyticsDevicePerformance](../api/devicemanagement-list-userexperienceanalyticsdeviceperformance.md)|[userExperienceAnalyticsDevicePerformance](../resources/userexperienceanalyticsdeviceperformance.md) collection|Get the userExperienceAnalyticsDevicePerformances from the userExperienceAnalyticsDevicePerformance navigation property.|
|[Create userExperienceAnalyticsDevicePerformance](../api/devicemanagement-post-userexperienceanalyticsdeviceperformance.md)|[userExperienceAnalyticsDevicePerformance](../resources/userexperienceanalyticsdeviceperformance.md)|Create a new userExperienceAnalyticsDevicePerformance object.|
|[Delete userExperienceAnalyticsDevicePerformance](../api/devicemanagement-delete-userexperienceanalyticsdeviceperformance.md)|None|Delete a [userExperienceAnalyticsDevicePerformance](../resources/userexperienceanalyticsdeviceperformance.md) object.|
|[Update userExperienceAnalyticsDevicePerformance](../api/devicemanagement-update-userexperienceanalyticsdeviceperformance.md)|[userExperienceAnalyticsDevicePerformance](../resources/userexperienceanalyticsdeviceperformance.md)|Update the properties of a userExperienceAnalyticsDevicePerformance object.|
|[Get userExperienceAnalyticsDevicePerformance](../api/userexperienceanalyticsdeviceperformance-get.md)|[userExperienceAnalyticsDevicePerformance](../resources/userexperienceanalyticsdeviceperformance.md)|Read the properties and relationships of a [userExperienceAnalyticsDevicePerformance](../resources/userexperienceanalyticsdeviceperformance.md) object.|
|[List userExperienceAnalyticsRegressionSummary](../api/devicemanagement-list-userexperienceanalyticsregressionsummary.md)|[userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md) collection|Get the userExperienceAnalyticsRegressionSummaries from the userExperienceAnalyticsRegressionSummary navigation property.|
|[Create userExperienceAnalyticsRegressionSummary](../api/devicemanagement-post-userexperienceanalyticsregressionsummary.md)|[userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md)|Create a new userExperienceAnalyticsRegressionSummary object.|
|[Delete userExperienceAnalyticsRegressionSummary](../api/devicemanagement-delete-userexperienceanalyticsregressionsummary.md)|None|Delete a [userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md) object.|
|[Update userExperienceAnalyticsRegressionSummary](../api/devicemanagement-update-userexperienceanalyticsregressionsummary.md)|[userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md)|Update the properties of a userExperienceAnalyticsRegressionSummary object.|
|[Get userExperienceAnalyticsRegressionSummary](../api/userexperienceanalyticsregressionsummary-get.md)|[userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md)|Read the properties and relationships of a [userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md) object.|
|[List userExperienceAnalyticsDeviceStartupHistory](../api/devicemanagement-list-userexperienceanalyticsdevicestartuphistory.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/userexperienceanalyticsdevicestartuphistory.md) collection|Get the userExperienceAnalyticsDeviceStartupHistories from the userExperienceAnalyticsDeviceStartupHistory navigation property.|
|[Create userExperienceAnalyticsDeviceStartupHistory](../api/devicemanagement-post-userexperienceanalyticsdevicestartuphistory.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/userexperienceanalyticsdevicestartuphistory.md)|Create a new userExperienceAnalyticsDeviceStartupHistory object.|
|[Delete userExperienceAnalyticsDeviceStartupHistory](../api/devicemanagement-delete-userexperienceanalyticsdevicestartuphistory.md)|None|Delete a [userExperienceAnalyticsDeviceStartupHistory](../resources/userexperienceanalyticsdevicestartuphistory.md) object.|
|[Update userExperienceAnalyticsDeviceStartupHistory](../api/devicemanagement-update-userexperienceanalyticsdevicestartuphistory.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/userexperienceanalyticsdevicestartuphistory.md)|Update the properties of a userExperienceAnalyticsDeviceStartupHistory object.|
|[Get userExperienceAnalyticsDeviceStartupHistory](../api/userexperienceanalyticsdevicestartuphistory-get.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/userexperienceanalyticsdevicestartuphistory.md)|Read the properties and relationships of a [userExperienceAnalyticsDeviceStartupHistory](../resources/userexperienceanalyticsdevicestartuphistory.md) object.|
|[List userExperienceAnalyticsDeviceStartupProcesses](../api/devicemanagement-list-userexperienceanalyticsdevicestartupprocesses.md)|[userExperienceAnalyticsDeviceStartupProcess](../resources/userexperienceanalyticsdevicestartupprocess.md) collection|Get the userExperienceAnalyticsDeviceStartupProcesses from the userExperienceAnalyticsDeviceStartupProcesses navigation property.|
|[Create userExperienceAnalyticsDeviceStartupProcesses](../api/devicemanagement-post-userexperienceanalyticsdevicestartupprocesses.md)|[userExperienceAnalyticsDeviceStartupProcess](../resources/userexperienceanalyticsdevicestartupprocess.md)|Create a new userExperienceAnalyticsDeviceStartupProcesses object.|
|[Delete userExperienceAnalyticsDeviceStartupProcesses](../api/devicemanagement-delete-userexperienceanalyticsdevicestartupprocesses.md)|None|Delete a [userExperienceAnalyticsDeviceStartupProcess](../resources/userexperienceanalyticsdevicestartupprocess.md) object.|
|[Update userExperienceAnalyticsDeviceStartupProcesses](../api/devicemanagement-update-userexperienceanalyticsdevicestartupprocesses.md)|[userExperienceAnalyticsDeviceStartupProcess](../resources/userexperienceanalyticsdevicestartupprocess.md)|Update the properties of a userExperienceAnalyticsDeviceStartupProcesses object.|
|[Get userExperienceAnalyticsDeviceStartupProcess](../api/userexperienceanalyticsdevicestartupprocess-get.md)|[userExperienceAnalyticsDeviceStartupProcess](../resources/userexperienceanalyticsdevicestartupprocess.md)|Read the properties and relationships of a [userExperienceAnalyticsDeviceStartupProcess](../resources/userexperienceanalyticsdevicestartupprocess.md) object.|
|[List userExperienceAnalyticsDeviceStartupProcessPerformance](../api/devicemanagement-list-userexperienceanalyticsdevicestartupprocessperformance.md)|[userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/userexperienceanalyticsdevicestartupprocessperformance.md) collection|Get the userExperienceAnalyticsDeviceStartupProcessPerformances from the userExperienceAnalyticsDeviceStartupProcessPerformance navigation property.|
|[Create userExperienceAnalyticsDeviceStartupProcessPerformance](../api/devicemanagement-post-userexperienceanalyticsdevicestartupprocessperformance.md)|[userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/userexperienceanalyticsdevicestartupprocessperformance.md)|Create a new userExperienceAnalyticsDeviceStartupProcessPerformance object.|
|[Delete userExperienceAnalyticsDeviceStartupProcessPerformance](../api/devicemanagement-delete-userexperienceanalyticsdevicestartupprocessperformance.md)|None|Delete a [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/userexperienceanalyticsdevicestartupprocessperformance.md) object.|
|[Update userExperienceAnalyticsDeviceStartupProcessPerformance](../api/devicemanagement-update-userexperienceanalyticsdevicestartupprocessperformance.md)|[userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/userexperienceanalyticsdevicestartupprocessperformance.md)|Update the properties of a userExperienceAnalyticsDeviceStartupProcessPerformance object.|
|[Get userExperienceAnalyticsDeviceStartupProcessPerformance](../api/userexperienceanalyticsdevicestartupprocessperformance-get.md)|[userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/userexperienceanalyticsdevicestartupprocessperformance.md)|Read the properties and relationships of a [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/userexperienceanalyticsdevicestartupprocessperformance.md) object.|
|[List userExperienceAnalyticsScoreHistory](../api/devicemanagement-list-userexperienceanalyticsscorehistory.md)|[userExperienceAnalyticsScoreHistory](../resources/userexperienceanalyticsscorehistory.md) collection|Get the userExperienceAnalyticsScoreHistories from the userExperienceAnalyticsScoreHistory navigation property.|
|[Create userExperienceAnalyticsScoreHistory](../api/devicemanagement-post-userexperienceanalyticsscorehistory.md)|[userExperienceAnalyticsScoreHistory](../resources/userexperienceanalyticsscorehistory.md)|Create a new userExperienceAnalyticsScoreHistory object.|
|[Delete userExperienceAnalyticsScoreHistory](../api/devicemanagement-delete-userexperienceanalyticsscorehistory.md)|None|Delete a [userExperienceAnalyticsScoreHistory](../resources/userexperienceanalyticsscorehistory.md) object.|
|[Update userExperienceAnalyticsScoreHistory](../api/devicemanagement-update-userexperienceanalyticsscorehistory.md)|[userExperienceAnalyticsScoreHistory](../resources/userexperienceanalyticsscorehistory.md)|Update the properties of a userExperienceAnalyticsScoreHistory object.|
|[Get userExperienceAnalyticsScoreHistory](../api/userexperienceanalyticsscorehistory-get.md)|[userExperienceAnalyticsScoreHistory](../resources/userexperienceanalyticsscorehistory.md)|Read the properties and relationships of a [userExperienceAnalyticsScoreHistory](../resources/userexperienceanalyticsscorehistory.md) object.|
|[List derivedCredentials](../api/devicemanagement-list-derivedcredentials.md)|[deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) collection|Get the deviceManagementDerivedCredentialSettings from the derivedCredentials navigation property.|
|[Create derivedCredentials](../api/devicemanagement-post-derivedcredentials.md)|[deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md)|Create a new derivedCredentials object.|
|[Delete derivedCredentials](../api/devicemanagement-delete-derivedcredentials.md)|None|Delete a [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) object.|
|[Update derivedCredentials](../api/devicemanagement-update-derivedcredentials.md)|[deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md)|Update the properties of a derivedCredentials object.|
|[Get deviceManagementDerivedCredentialSettings](../api/devicemanagementderivedcredentialsettings-get.md)|[deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md)|Read the properties and relationships of a [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) object.|
|[List windowsAutopilotSettings](../api/devicemanagement-list-windowsautopilotsettings.md)|[windowsAutopilotSettings](../resources/windowsautopilotsettings.md) collection|Get the windowsAutopilotSettings from the windowsAutopilotSettings navigation property.|
|[Create windowsAutopilotSettings](../api/devicemanagement-post-windowsautopilotsettings.md)|[windowsAutopilotSettings](../resources/windowsautopilotsettings.md)|Create a new windowsAutopilotSettings object.|
|[Delete windowsAutopilotSettings](../api/devicemanagement-delete-windowsautopilotsettings.md)|None|Delete a [windowsAutopilotSettings](../resources/windowsautopilotsettings.md) object.|
|[Update windowsAutopilotSettings](../api/devicemanagement-update-windowsautopilotsettings.md)|[windowsAutopilotSettings](../resources/windowsautopilotsettings.md)|Update the properties of a windowsAutopilotSettings object.|
|[Get windowsAutopilotSettings](../api/windowsautopilotsettings-get.md)|[windowsAutopilotSettings](../resources/windowsautopilotsettings.md)|Read the properties and relationships of a [windowsAutopilotSettings](../resources/windowsautopilotsettings.md) object.|
|[List windowsAutopilotDeviceIdentities](../api/devicemanagement-list-windowsautopilotdeviceidentities.md)|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) collection|Get the windowsAutopilotDeviceIdentities from the windowsAutopilotDeviceIdentities navigation property.|
|[Create windowsAutopilotDeviceIdentities](../api/devicemanagement-post-windowsautopilotdeviceidentities.md)|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md)|Create a new windowsAutopilotDeviceIdentities object.|
|[Delete windowsAutopilotDeviceIdentities](../api/devicemanagement-delete-windowsautopilotdeviceidentities.md)|None|Delete a [windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) object.|
|[Update windowsAutopilotDeviceIdentities](../api/devicemanagement-update-windowsautopilotdeviceidentities.md)|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md)|Update the properties of a windowsAutopilotDeviceIdentities object.|
|[Get windowsAutopilotDeviceIdentity](../api/windowsautopilotdeviceidentity-get.md)|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md)|Read the properties and relationships of a [windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) object.|
|[List windowsAutopilotDeploymentProfiles](../api/devicemanagement-list-windowsautopilotdeploymentprofiles.md)|[windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md) collection|Get the windowsAutopilotDeploymentProfiles from the windowsAutopilotDeploymentProfiles navigation property.|
|[Create windowsAutopilotDeploymentProfiles](../api/devicemanagement-post-windowsautopilotdeploymentprofiles.md)|[windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md)|Create a new windowsAutopilotDeploymentProfiles object.|
|[Delete windowsAutopilotDeploymentProfiles](../api/devicemanagement-delete-windowsautopilotdeploymentprofiles.md)|None|Delete a [windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md) object.|
|[Update windowsAutopilotDeploymentProfiles](../api/devicemanagement-update-windowsautopilotdeploymentprofiles.md)|[windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md)|Update the properties of a windowsAutopilotDeploymentProfiles object.|
|[Get windowsAutopilotDeploymentProfile](../api/windowsautopilotdeploymentprofile-get.md)|[windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md)|Read the properties and relationships of a [windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md) object.|
|[List importedDeviceIdentities](../api/devicemanagement-list-importeddeviceidentities.md)|[importedDeviceIdentity](../resources/importeddeviceidentity.md) collection|Get the importedDeviceIdentities from the importedDeviceIdentities navigation property.|
|[Create importedDeviceIdentities](../api/devicemanagement-post-importeddeviceidentities.md)|[importedDeviceIdentity](../resources/importeddeviceidentity.md)|Create a new importedDeviceIdentities object.|
|[Delete importedDeviceIdentities](../api/devicemanagement-delete-importeddeviceidentities.md)|None|Delete an [importedDeviceIdentity](../resources/importeddeviceidentity.md) object.|
|[Update importedDeviceIdentities](../api/devicemanagement-update-importeddeviceidentities.md)|[importedDeviceIdentity](../resources/importeddeviceidentity.md)|Update the properties of an importedDeviceIdentities object.|
|[Get importedDeviceIdentity](../api/importeddeviceidentity-get.md)|[importedDeviceIdentity](../resources/importeddeviceidentity.md)|Read the properties and relationships of an [importedDeviceIdentity](../resources/importeddeviceidentity.md) object.|
|[List depOnboardingSettings](../api/devicemanagement-list-deponboardingsettings.md)|[depOnboardingSetting](../resources/deponboardingsetting.md) collection|Get the depOnboardingSettings from the depOnboardingSettings navigation property.|
|[Create depOnboardingSettings](../api/devicemanagement-post-deponboardingsettings.md)|[depOnboardingSetting](../resources/deponboardingsetting.md)|Create a new depOnboardingSettings object.|
|[Delete depOnboardingSettings](../api/devicemanagement-delete-deponboardingsettings.md)|None|Delete a [depOnboardingSetting](../resources/deponboardingsetting.md) object.|
|[Update depOnboardingSettings](../api/devicemanagement-update-deponboardingsettings.md)|[depOnboardingSetting](../resources/deponboardingsetting.md)|Update the properties of a depOnboardingSettings object.|
|[Get depOnboardingSetting](../api/deponboardingsetting-get.md)|[depOnboardingSetting](../resources/deponboardingsetting.md)|Read the properties and relationships of a [depOnboardingSetting](../resources/deponboardingsetting.md) object.|
|[List importedWindowsAutopilotDeviceIdentities](../api/devicemanagement-list-importedwindowsautopilotdeviceidentities.md)|[importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md) collection|Get the importedWindowsAutopilotDeviceIdentities from the importedWindowsAutopilotDeviceIdentities navigation property.|
|[Create importedWindowsAutopilotDeviceIdentities](../api/devicemanagement-post-importedwindowsautopilotdeviceidentities.md)|[importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md)|Create a new importedWindowsAutopilotDeviceIdentities object.|
|[Delete importedWindowsAutopilotDeviceIdentities](../api/devicemanagement-delete-importedwindowsautopilotdeviceidentities.md)|None|Delete an [importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md) object.|
|[Update importedWindowsAutopilotDeviceIdentities](../api/devicemanagement-update-importedwindowsautopilotdeviceidentities.md)|[importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md)|Update the properties of an importedWindowsAutopilotDeviceIdentities object.|
|[Get importedWindowsAutopilotDeviceIdentity](../api/importedwindowsautopilotdeviceidentity-get.md)|[importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md)|Read the properties and relationships of an [importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md) object.|
|[List appleUserInitiatedEnrollmentProfiles](../api/devicemanagement-list-appleuserinitiatedenrollmentprofiles.md)|[appleUserInitiatedEnrollmentProfile](../resources/appleuserinitiatedenrollmentprofile.md) collection|Get the appleUserInitiatedEnrollmentProfiles from the appleUserInitiatedEnrollmentProfiles navigation property.|
|[Create appleUserInitiatedEnrollmentProfiles](../api/devicemanagement-post-appleuserinitiatedenrollmentprofiles.md)|[appleUserInitiatedEnrollmentProfile](../resources/appleuserinitiatedenrollmentprofile.md)|Create a new appleUserInitiatedEnrollmentProfiles object.|
|[Delete appleUserInitiatedEnrollmentProfiles](../api/devicemanagement-delete-appleuserinitiatedenrollmentprofiles.md)|None|Delete an [appleUserInitiatedEnrollmentProfile](../resources/appleuserinitiatedenrollmentprofile.md) object.|
|[Update appleUserInitiatedEnrollmentProfiles](../api/devicemanagement-update-appleuserinitiatedenrollmentprofiles.md)|[appleUserInitiatedEnrollmentProfile](../resources/appleuserinitiatedenrollmentprofile.md)|Update the properties of an appleUserInitiatedEnrollmentProfiles object.|
|[Get appleUserInitiatedEnrollmentProfile](../api/appleuserinitiatedenrollmentprofile-get.md)|[appleUserInitiatedEnrollmentProfile](../resources/appleuserinitiatedenrollmentprofile.md)|Read the properties and relationships of an [appleUserInitiatedEnrollmentProfile](../resources/appleuserinitiatedenrollmentprofile.md) object.|
|[List managementConditions](../api/devicemanagement-list-managementconditions.md)|[managementCondition](../resources/managementcondition.md) collection|Get the managementConditions from the managementConditions navigation property.|
|[Create managementConditions](../api/devicemanagement-post-managementconditions.md)|[managementCondition](../resources/managementcondition.md)|Create a new managementConditions object.|
|[Delete managementConditions](../api/devicemanagement-delete-managementconditions.md)|None|Delete a [managementCondition](../resources/managementcondition.md) object.|
|[Update managementConditions](../api/devicemanagement-update-managementconditions.md)|[managementCondition](../resources/managementcondition.md)|Update the properties of a managementConditions object.|
|[Get managementCondition](../api/managementcondition-get.md)|[managementCondition](../resources/managementcondition.md)|Read the properties and relationships of a [managementCondition](../resources/managementcondition.md) object.|
|[List managementConditionStatements](../api/devicemanagement-list-managementconditionstatements.md)|[managementConditionStatement](../resources/managementconditionstatement.md) collection|Get the managementConditionStatements from the managementConditionStatements navigation property.|
|[Create managementConditionStatements](../api/devicemanagement-post-managementconditionstatements.md)|[managementConditionStatement](../resources/managementconditionstatement.md)|Create a new managementConditionStatements object.|
|[Delete managementConditionStatements](../api/devicemanagement-delete-managementconditionstatements.md)|None|Delete a [managementConditionStatement](../resources/managementconditionstatement.md) object.|
|[Update managementConditionStatements](../api/devicemanagement-update-managementconditionstatements.md)|[managementConditionStatement](../resources/managementconditionstatement.md)|Update the properties of a managementConditionStatements object.|
|[Get managementConditionStatement](../api/managementconditionstatement-get.md)|[managementConditionStatement](../resources/managementconditionstatement.md)|Read the properties and relationships of a [managementConditionStatement](../resources/managementconditionstatement.md) object.|
|[List groupPolicyObjectFiles](../api/devicemanagement-list-grouppolicyobjectfiles.md)|[groupPolicyObjectFile](../resources/grouppolicyobjectfile.md) collection|Get the groupPolicyObjectFiles from the groupPolicyObjectFiles navigation property.|
|[Create groupPolicyObjectFiles](../api/devicemanagement-post-grouppolicyobjectfiles.md)|[groupPolicyObjectFile](../resources/grouppolicyobjectfile.md)|Create a new groupPolicyObjectFiles object.|
|[Delete groupPolicyObjectFiles](../api/devicemanagement-delete-grouppolicyobjectfiles.md)|None|Delete a [groupPolicyObjectFile](../resources/grouppolicyobjectfile.md) object.|
|[Update groupPolicyObjectFiles](../api/devicemanagement-update-grouppolicyobjectfiles.md)|[groupPolicyObjectFile](../resources/grouppolicyobjectfile.md)|Update the properties of a groupPolicyObjectFiles object.|
|[Get groupPolicyObjectFile](../api/grouppolicyobjectfile-get.md)|[groupPolicyObjectFile](../resources/grouppolicyobjectfile.md)|Read the properties and relationships of a [groupPolicyObjectFile](../resources/grouppolicyobjectfile.md) object.|
|[List groupPolicyMigrationReports](../api/devicemanagement-list-grouppolicymigrationreports.md)|[groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) collection|Get the groupPolicyMigrationReports from the groupPolicyMigrationReports navigation property.|
|[Create groupPolicyMigrationReports](../api/devicemanagement-post-grouppolicymigrationreports.md)|[groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md)|Create a new groupPolicyMigrationReports object.|
|[Delete groupPolicyMigrationReports](../api/devicemanagement-delete-grouppolicymigrationreports.md)|None|Delete a [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) object.|
|[Update groupPolicyMigrationReports](../api/devicemanagement-update-grouppolicymigrationreports.md)|[groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md)|Update the properties of a groupPolicyMigrationReports object.|
|[Get groupPolicyMigrationReport](../api/grouppolicymigrationreport-get.md)|[groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md)|Read the properties and relationships of a [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) object.|
|[List groupPolicyConfigurations](../api/devicemanagement-list-grouppolicyconfigurations.md)|[groupPolicyConfiguration](../resources/grouppolicyconfiguration.md) collection|Get the groupPolicyConfigurations from the groupPolicyConfigurations navigation property.|
|[Create groupPolicyConfigurations](../api/devicemanagement-post-grouppolicyconfigurations.md)|[groupPolicyConfiguration](../resources/grouppolicyconfiguration.md)|Create a new groupPolicyConfigurations object.|
|[Delete groupPolicyConfigurations](../api/devicemanagement-delete-grouppolicyconfigurations.md)|None|Delete a [groupPolicyConfiguration](../resources/grouppolicyconfiguration.md) object.|
|[Update groupPolicyConfigurations](../api/devicemanagement-update-grouppolicyconfigurations.md)|[groupPolicyConfiguration](../resources/grouppolicyconfiguration.md)|Update the properties of a groupPolicyConfigurations object.|
|[Get groupPolicyConfiguration](../api/grouppolicyconfiguration-get.md)|[groupPolicyConfiguration](../resources/grouppolicyconfiguration.md)|Read the properties and relationships of a [groupPolicyConfiguration](../resources/grouppolicyconfiguration.md) object.|
|[List groupPolicyCategories](../api/devicemanagement-list-grouppolicycategories.md)|[groupPolicyCategory](../resources/grouppolicycategory.md) collection|Get the groupPolicyCategories from the groupPolicyCategories navigation property.|
|[Create groupPolicyCategories](../api/devicemanagement-post-grouppolicycategories.md)|[groupPolicyCategory](../resources/grouppolicycategory.md)|Create a new groupPolicyCategories object.|
|[Delete groupPolicyCategories](../api/devicemanagement-delete-grouppolicycategories.md)|None|Delete a [groupPolicyCategory](../resources/grouppolicycategory.md) object.|
|[Update groupPolicyCategories](../api/devicemanagement-update-grouppolicycategories.md)|[groupPolicyCategory](../resources/grouppolicycategory.md)|Update the properties of a groupPolicyCategories object.|
|[Get groupPolicyCategory](../api/grouppolicycategory-get.md)|[groupPolicyCategory](../resources/grouppolicycategory.md)|Read the properties and relationships of a [groupPolicyCategory](../resources/grouppolicycategory.md) object.|
|[List groupPolicyDefinitions](../api/devicemanagement-list-grouppolicydefinitions.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md) collection|Get the groupPolicyDefinitions from the groupPolicyDefinitions navigation property.|
|[Create groupPolicyDefinitions](../api/devicemanagement-post-grouppolicydefinitions.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Create a new groupPolicyDefinitions object.|
|[Delete groupPolicyDefinitions](../api/devicemanagement-delete-grouppolicydefinitions.md)|None|Delete a [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|
|[Update groupPolicyDefinitions](../api/devicemanagement-update-grouppolicydefinitions.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Update the properties of a groupPolicyDefinitions object.|
|[Get groupPolicyDefinition](../api/grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Read the properties and relationships of a [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|
|[List groupPolicyDefinitionFiles](../api/devicemanagement-list-grouppolicydefinitionfiles.md)|[groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) collection|Get the groupPolicyDefinitionFiles from the groupPolicyDefinitionFiles navigation property.|
|[Create groupPolicyDefinitionFiles](../api/devicemanagement-post-grouppolicydefinitionfiles.md)|[groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|Create a new groupPolicyDefinitionFiles object.|
|[Delete groupPolicyDefinitionFiles](../api/devicemanagement-delete-grouppolicydefinitionfiles.md)|None|Delete a [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) object.|
|[Update groupPolicyDefinitionFiles](../api/devicemanagement-update-grouppolicydefinitionfiles.md)|[groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|Update the properties of a groupPolicyDefinitionFiles object.|
|[Get groupPolicyDefinitionFile](../api/grouppolicydefinitionfile-get.md)|[groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|Read the properties and relationships of a [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) object.|
|[List groupPolicyUploadedDefinitionFiles](../api/devicemanagement-list-grouppolicyuploadeddefinitionfiles.md)|[groupPolicyUploadedDefinitionFile](../resources/grouppolicyuploadeddefinitionfile.md) collection|Get the groupPolicyUploadedDefinitionFiles from the groupPolicyUploadedDefinitionFiles navigation property.|
|[Create groupPolicyUploadedDefinitionFiles](../api/devicemanagement-post-grouppolicyuploadeddefinitionfiles.md)|[groupPolicyUploadedDefinitionFile](../resources/grouppolicyuploadeddefinitionfile.md)|Create a new groupPolicyUploadedDefinitionFiles object.|
|[Delete groupPolicyUploadedDefinitionFiles](../api/devicemanagement-delete-grouppolicyuploadeddefinitionfiles.md)|None|Delete a [groupPolicyUploadedDefinitionFile](../resources/grouppolicyuploadeddefinitionfile.md) object.|
|[Update groupPolicyUploadedDefinitionFiles](../api/devicemanagement-update-grouppolicyuploadeddefinitionfiles.md)|[groupPolicyUploadedDefinitionFile](../resources/grouppolicyuploadeddefinitionfile.md)|Update the properties of a groupPolicyUploadedDefinitionFiles object.|
|[Get groupPolicyUploadedDefinitionFile](../api/grouppolicyuploadeddefinitionfile-get.md)|[groupPolicyUploadedDefinitionFile](../resources/grouppolicyuploadeddefinitionfile.md)|Read the properties and relationships of a [groupPolicyUploadedDefinitionFile](../resources/grouppolicyuploadeddefinitionfile.md) object.|
|[List notificationMessageTemplates](../api/devicemanagement-list-notificationmessagetemplates.md)|[notificationMessageTemplate](../resources/notificationmessagetemplate.md) collection|Get the notificationMessageTemplates from the notificationMessageTemplates navigation property.|
|[Create notificationMessageTemplates](../api/devicemanagement-post-notificationmessagetemplates.md)|[notificationMessageTemplate](../resources/notificationmessagetemplate.md)|Create a new notificationMessageTemplates object.|
|[Delete notificationMessageTemplates](../api/devicemanagement-delete-notificationmessagetemplates.md)|None|Delete a [notificationMessageTemplate](../resources/notificationmessagetemplate.md) object.|
|[Update notificationMessageTemplates](../api/devicemanagement-update-notificationmessagetemplates.md)|[notificationMessageTemplate](../resources/notificationmessagetemplate.md)|Update the properties of a notificationMessageTemplates object.|
|[Get notificationMessageTemplate](../api/notificationmessagetemplate-get.md)|[notificationMessageTemplate](../resources/notificationmessagetemplate.md)|Read the properties and relationships of a [notificationMessageTemplate](../resources/notificationmessagetemplate.md) object.|
|[List domainJoinConnectors](../api/devicemanagement-list-domainjoinconnectors.md)|[deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md) collection|Get the deviceManagementDomainJoinConnectors from the domainJoinConnectors navigation property.|
|[Create domainJoinConnectors](../api/devicemanagement-post-domainjoinconnectors.md)|[deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md)|Create a new domainJoinConnectors object.|
|[Delete domainJoinConnectors](../api/devicemanagement-delete-domainjoinconnectors.md)|None|Delete a [deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md) object.|
|[Update domainJoinConnectors](../api/devicemanagement-update-domainjoinconnectors.md)|[deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md)|Update the properties of a domainJoinConnectors object.|
|[Get deviceManagementDomainJoinConnector](../api/devicemanagementdomainjoinconnector-get.md)|[deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md)|Read the properties and relationships of a [deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md) object.|
|[List roleDefinitions](../api/devicemanagement-list-roledefinitions.md)|[roleDefinition](../resources/roledefinition.md) collection|Get the roleDefinitions from the roleDefinitions navigation property.|
|[Create roleDefinitions](../api/devicemanagement-post-roledefinitions.md)|[roleDefinition](../resources/roledefinition.md)|Create a new roleDefinitions object.|
|[Delete roleDefinitions](../api/devicemanagement-delete-roledefinitions.md)|None|Delete a [roleDefinition](../resources/roledefinition.md) object.|
|[Update roleDefinitions](../api/devicemanagement-update-roledefinitions.md)|[roleDefinition](../resources/roledefinition.md)|Update the properties of a roleDefinitions object.|
|[Get roleDefinition](../api/roledefinition-get.md)|[roleDefinition](../resources/roledefinition.md)|Read the properties and relationships of a [roleDefinition](../resources/roledefinition.md) object.|
|[List roleAssignments](../api/devicemanagement-list-roleassignments.md)|[deviceAndAppManagementRoleAssignment](../resources/deviceandappmanagementroleassignment.md) collection|Get the deviceAndAppManagementRoleAssignments from the roleAssignments navigation property.|
|[Create roleAssignments](../api/devicemanagement-post-roleassignments.md)|[deviceAndAppManagementRoleAssignment](../resources/deviceandappmanagementroleassignment.md)|Create a new roleAssignments object.|
|[Delete roleAssignments](../api/devicemanagement-delete-roleassignments.md)|None|Delete a [deviceAndAppManagementRoleAssignment](../resources/deviceandappmanagementroleassignment.md) object.|
|[Update roleAssignments](../api/devicemanagement-update-roleassignments.md)|[deviceAndAppManagementRoleAssignment](../resources/deviceandappmanagementroleassignment.md)|Update the properties of a roleAssignments object.|
|[Get deviceAndAppManagementRoleAssignment](../api/deviceandappmanagementroleassignment-get.md)|[deviceAndAppManagementRoleAssignment](../resources/deviceandappmanagementroleassignment.md)|Read the properties and relationships of a [deviceAndAppManagementRoleAssignment](../resources/deviceandappmanagementroleassignment.md) object.|
|[List roleScopeTags](../api/devicemanagement-list-rolescopetags.md)|[roleScopeTag](../resources/rolescopetag.md) collection|Get the roleScopeTags from the roleScopeTags navigation property.|
|[Create roleScopeTags](../api/devicemanagement-post-rolescopetags.md)|[roleScopeTag](../resources/rolescopetag.md)|Create a new roleScopeTags object.|
|[Delete roleScopeTags](../api/devicemanagement-delete-rolescopetags.md)|None|Delete a [roleScopeTag](../resources/rolescopetag.md) object.|
|[Update roleScopeTags](../api/devicemanagement-update-rolescopetags.md)|[roleScopeTag](../resources/rolescopetag.md)|Update the properties of a roleScopeTags object.|
|[Get roleScopeTag](../api/rolescopetag-get.md)|[roleScopeTag](../resources/rolescopetag.md)|Read the properties and relationships of a [roleScopeTag](../resources/rolescopetag.md) object.|
|[List resourceOperations](../api/devicemanagement-list-resourceoperations.md)|[resourceOperation](../resources/resourceoperation.md) collection|Get the resourceOperations from the resourceOperations navigation property.|
|[Create resourceOperations](../api/devicemanagement-post-resourceoperations.md)|[resourceOperation](../resources/resourceoperation.md)|Create a new resourceOperations object.|
|[Delete resourceOperations](../api/devicemanagement-delete-resourceoperations.md)|None|Delete a [resourceOperation](../resources/resourceoperation.md) object.|
|[Update resourceOperations](../api/devicemanagement-update-resourceoperations.md)|[resourceOperation](../resources/resourceoperation.md)|Update the properties of a resourceOperations object.|
|[Get resourceOperation](../api/resourceoperation-get.md)|[resourceOperation](../resources/resourceoperation.md)|Read the properties and relationships of a [resourceOperation](../resources/resourceoperation.md) object.|
|[List remoteAssistancePartners](../api/devicemanagement-list-remoteassistancepartners.md)|[remoteAssistancePartner](../resources/remoteassistancepartner.md) collection|Get the remoteAssistancePartners from the remoteAssistancePartners navigation property.|
|[Create remoteAssistancePartners](../api/devicemanagement-post-remoteassistancepartners.md)|[remoteAssistancePartner](../resources/remoteassistancepartner.md)|Create a new remoteAssistancePartners object.|
|[Delete remoteAssistancePartners](../api/devicemanagement-delete-remoteassistancepartners.md)|None|Delete a [remoteAssistancePartner](../resources/remoteassistancepartner.md) object.|
|[Update remoteAssistancePartners](../api/devicemanagement-update-remoteassistancepartners.md)|[remoteAssistancePartner](../resources/remoteassistancepartner.md)|Update the properties of a remoteAssistancePartners object.|
|[Get remoteAssistancePartner](../api/remoteassistancepartner-get.md)|[remoteAssistancePartner](../resources/remoteassistancepartner.md)|Read the properties and relationships of a [remoteAssistancePartner](../resources/remoteassistancepartner.md) object.|
|[List reports](../api/devicemanagement-list-reports.md)|[deviceManagementReports](../resources/devicemanagementreports.md) collection|Get the deviceManagementReports from the reports navigation property.|
|[Create reports](../api/devicemanagement-post-reports.md)|[deviceManagementReports](../resources/devicemanagementreports.md)|Create a new reports object.|
|[Delete reports](../api/devicemanagement-delete-reports.md)|None|Delete a [deviceManagementReports](../resources/devicemanagementreports.md) object.|
|[Update reports](../api/devicemanagement-update-reports.md)|[deviceManagementReports](../resources/devicemanagementreports.md)|Update the properties of a reports object.|
|[Get deviceManagementReports](../api/devicemanagementreports-get.md)|[deviceManagementReports](../resources/devicemanagementreports.md)|Read the properties and relationships of a [deviceManagementReports](../resources/devicemanagementreports.md) object.|
|[List telecomExpenseManagementPartners](../api/devicemanagement-list-telecomexpensemanagementpartners.md)|[telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) collection|Get the telecomExpenseManagementPartners from the telecomExpenseManagementPartners navigation property.|
|[Create telecomExpenseManagementPartners](../api/devicemanagement-post-telecomexpensemanagementpartners.md)|[telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md)|Create a new telecomExpenseManagementPartners object.|
|[Delete telecomExpenseManagementPartners](../api/devicemanagement-delete-telecomexpensemanagementpartners.md)|None|Delete a [telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) object.|
|[Update telecomExpenseManagementPartners](../api/devicemanagement-update-telecomexpensemanagementpartners.md)|[telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md)|Update the properties of a telecomExpenseManagementPartners object.|
|[Get telecomExpenseManagementPartner](../api/telecomexpensemanagementpartner-get.md)|[telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md)|Read the properties and relationships of a [telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) object.|
|[List embeddedSIMActivationCodePools](../api/devicemanagement-list-embeddedsimactivationcodepools.md)|[embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md) collection|Get the embeddedSIMActivationCodePools from the embeddedSIMActivationCodePools navigation property.|
|[Create embeddedSIMActivationCodePools](../api/devicemanagement-post-embeddedsimactivationcodepools.md)|[embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md)|Create a new embeddedSIMActivationCodePools object.|
|[Delete embeddedSIMActivationCodePools](../api/devicemanagement-delete-embeddedsimactivationcodepools.md)|None|Delete an [embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md) object.|
|[Update embeddedSIMActivationCodePools](../api/devicemanagement-update-embeddedsimactivationcodepools.md)|[embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md)|Update the properties of an embeddedSIMActivationCodePools object.|
|[Get embeddedSIMActivationCodePool](../api/embeddedsimactivationcodepool-get.md)|[embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md)|Read the properties and relationships of an [embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md) object.|
|[List troubleshootingEvents](../api/devicemanagement-list-troubleshootingevents.md)|[deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md) collection|Get the deviceManagementTroubleshootingEvents from the troubleshootingEvents navigation property.|
|[Create troubleshootingEvents](../api/devicemanagement-post-troubleshootingevents.md)|[deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|Create a new troubleshootingEvents object.|
|[Delete troubleshootingEvents](../api/devicemanagement-delete-troubleshootingevents.md)|None|Delete a [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md) object.|
|[Update troubleshootingEvents](../api/devicemanagement-update-troubleshootingevents.md)|[deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|Update the properties of a troubleshootingEvents object.|
|[Get deviceManagementTroubleshootingEvent](../api/devicemanagementtroubleshootingevent-get.md)|[deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|Read the properties and relationships of a [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md) object.|
|[List autopilotEvents](../api/devicemanagement-list-autopilotevents.md)|[deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) collection|Get the deviceManagementAutopilotEvents from the autopilotEvents navigation property.|
|[Create autopilotEvents](../api/devicemanagement-post-autopilotevents.md)|[deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md)|Create a new autopilotEvents object.|
|[Delete autopilotEvents](../api/devicemanagement-delete-autopilotevents.md)|None|Delete an [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) object.|
|[Update autopilotEvents](../api/devicemanagement-update-autopilotevents.md)|[deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md)|Update the properties of an autopilotEvents object.|
|[Get deviceManagementAutopilotEvent](../api/devicemanagementautopilotevent-get.md)|[deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md)|Read the properties and relationships of a [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) object.|
|[List windowsFeatureUpdateProfiles](../api/devicemanagement-list-windowsfeatureupdateprofiles.md)|[windowsFeatureUpdateProfile](../resources/windowsfeatureupdateprofile.md) collection|Get the windowsFeatureUpdateProfiles from the windowsFeatureUpdateProfiles navigation property.|
|[Create windowsFeatureUpdateProfiles](../api/devicemanagement-post-windowsfeatureupdateprofiles.md)|[windowsFeatureUpdateProfile](../resources/windowsfeatureupdateprofile.md)|Create a new windowsFeatureUpdateProfiles object.|
|[Delete windowsFeatureUpdateProfiles](../api/devicemanagement-delete-windowsfeatureupdateprofiles.md)|None|Delete a [windowsFeatureUpdateProfile](../resources/windowsfeatureupdateprofile.md) object.|
|[Update windowsFeatureUpdateProfiles](../api/devicemanagement-update-windowsfeatureupdateprofiles.md)|[windowsFeatureUpdateProfile](../resources/windowsfeatureupdateprofile.md)|Update the properties of a windowsFeatureUpdateProfiles object.|
|[Get windowsFeatureUpdateProfile](../api/windowsfeatureupdateprofile-get.md)|[windowsFeatureUpdateProfile](../resources/windowsfeatureupdateprofile.md)|Read the properties and relationships of a [windowsFeatureUpdateProfile](../resources/windowsfeatureupdateprofile.md) object.|
|[List windowsInformationProtectionAppLearningSummaries](../api/devicemanagement-list-windowsinformationprotectionapplearningsummaries.md)|[windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md) collection|Get the windowsInformationProtectionAppLearningSummaries from the windowsInformationProtectionAppLearningSummaries navigation property.|
|[Create windowsInformationProtectionAppLearningSummaries](../api/devicemanagement-post-windowsinformationprotectionapplearningsummaries.md)|[windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md)|Create a new windowsInformationProtectionAppLearningSummaries object.|
|[Delete windowsInformationProtectionAppLearningSummaries](../api/devicemanagement-delete-windowsinformationprotectionapplearningsummaries.md)|None|Delete a [windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md) object.|
|[Update windowsInformationProtectionAppLearningSummaries](../api/devicemanagement-update-windowsinformationprotectionapplearningsummaries.md)|[windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md)|Update the properties of a windowsInformationProtectionAppLearningSummaries object.|
|[Get windowsInformationProtectionAppLearningSummary](../api/windowsinformationprotectionapplearningsummary-get.md)|[windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md)|Read the properties and relationships of a [windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md) object.|
|[List windowsInformationProtectionNetworkLearningSummaries](../api/devicemanagement-list-windowsinformationprotectionnetworklearningsummaries.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md) collection|Get the windowsInformationProtectionNetworkLearningSummaries from the windowsInformationProtectionNetworkLearningSummaries navigation property.|
|[Create windowsInformationProtectionNetworkLearningSummaries](../api/devicemanagement-post-windowsinformationprotectionnetworklearningsummaries.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md)|Create a new windowsInformationProtectionNetworkLearningSummaries object.|
|[Delete windowsInformationProtectionNetworkLearningSummaries](../api/devicemanagement-delete-windowsinformationprotectionnetworklearningsummaries.md)|None|Delete a [windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md) object.|
|[Update windowsInformationProtectionNetworkLearningSummaries](../api/devicemanagement-update-windowsinformationprotectionnetworklearningsummaries.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md)|Update the properties of a windowsInformationProtectionNetworkLearningSummaries object.|
|[Get windowsInformationProtectionNetworkLearningSummary](../api/windowsinformationprotectionnetworklearningsummary-get.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md)|Read the properties and relationships of a [windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md) object.|
|[List intuneBrandingProfiles](../api/devicemanagement-list-intunebrandingprofiles.md)|[intuneBrandingProfile](../resources/intunebrandingprofile.md) collection|Get the intuneBrandingProfiles from the intuneBrandingProfiles navigation property.|
|[Create intuneBrandingProfiles](../api/devicemanagement-post-intunebrandingprofiles.md)|[intuneBrandingProfile](../resources/intunebrandingprofile.md)|Create a new intuneBrandingProfiles object.|
|[Delete intuneBrandingProfiles](../api/devicemanagement-delete-intunebrandingprofiles.md)|None|Delete an [intuneBrandingProfile](../resources/intunebrandingprofile.md) object.|
|[Update intuneBrandingProfiles](../api/devicemanagement-update-intunebrandingprofiles.md)|[intuneBrandingProfile](../resources/intunebrandingprofile.md)|Update the properties of an intuneBrandingProfiles object.|
|[Get intuneBrandingProfile](../api/intunebrandingprofile-get.md)|[intuneBrandingProfile](../resources/intunebrandingprofile.md)|Read the properties and relationships of an [intuneBrandingProfile](../resources/intunebrandingprofile.md) object.|
|[List userPfxCertificates](../api/devicemanagement-list-userpfxcertificates.md)|[userPFXCertificate](../resources/userpfxcertificate.md) collection|Get the userPFXCertificates from the userPfxCertificates navigation property.|
|[Create userPfxCertificates](../api/devicemanagement-post-userpfxcertificates.md)|[userPFXCertificate](../resources/userpfxcertificate.md)|Create a new userPfxCertificates object.|
|[Delete userPfxCertificates](../api/devicemanagement-delete-userpfxcertificates.md)|None|Delete a [userPFXCertificate](../resources/userpfxcertificate.md) object.|
|[Update userPfxCertificates](../api/devicemanagement-update-userpfxcertificates.md)|[userPFXCertificate](../resources/userpfxcertificate.md)|Update the properties of a userPfxCertificates object.|
|[Get userPFXCertificate](../api/userpfxcertificate-get.md)|[userPFXCertificate](../resources/userpfxcertificate.md)|Read the properties and relationships of a [userPFXCertificate](../resources/userpfxcertificate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountMoveCompletionDateTime|DateTimeOffset|The date & time when tenant data moved between scaleunits.|
|adminConsent|[adminConsent](../resources/adminconsent.md)|Admin consent information.|
|deviceComplianceReportSummarizationDateTime|DateTimeOffset|The last requested time of device compliance reporting for this account. This property is read-only.|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/deviceprotectionoverview.md)|Device protection overview.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|intuneAccountId|Guid|Intune Account Id for given tenant|
|intuneBrand|[intuneBrand](../resources/intunebrand.md)|intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.|
|lastReportAggregationDateTime|DateTimeOffset|The last modified time of reporting for this account. This property is read-only.|
|legacyPcManangementEnabled|Boolean|The property to enable Non-MDM managed legacy PC management for this account. This property is read-only.|
|managedDeviceCleanupSettings|[managedDeviceCleanupSettings](../resources/manageddevicecleanupsettings.md)|Device cleanup rule|
|maximumDepTokens|Int32|Maximum number of dep tokens allowed per-tenant.|
|settings|[deviceManagementSettings](../resources/devicemanagementsettings.md)|Account level settings.|
|subscriptions|deviceManagementSubscriptions|Tenant's Subscription. Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.|
|subscriptionState|deviceManagementSubscriptionState|Tenant mobile device management subscription state. Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/windowsmalwareoverview.md)|Malware overview for windows devices.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|advancedThreatProtectionOnboardingStateSummary|[advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md)|The summary state of ATP onboarding state for this account.|
|androidDeviceOwnerEnrollmentProfiles|[androidDeviceOwnerEnrollmentProfile](../resources/androiddeviceownerenrollmentprofile.md) collection|Android device owner enrollment profile entities.|
|androidForWorkAppConfigurationSchemas|[androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md) collection|Android for Work app configuration schema entities.|
|androidForWorkEnrollmentProfiles|[androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) collection|Android for Work enrollment profile entities.|
|androidForWorkSettings|[androidForWorkSettings](../resources/androidforworksettings.md)|The singleton Android for Work settings entity.|
|androidManagedStoreAccountEnterpriseSettings|[androidManagedStoreAccountEnterpriseSettings](../resources/androidmanagedstoreaccountenterprisesettings.md)|The singleton Android managed store account enterprise settings entity.|
|androidManagedStoreAppConfigurationSchemas|[androidManagedStoreAppConfigurationSchema](../resources/androidmanagedstoreappconfigurationschema.md) collection|Android Enterprise app configuration schema entities.|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/applepushnotificationcertificate.md)|Apple push notification certificate.|
|appleUserInitiatedEnrollmentProfiles|[appleUserInitiatedEnrollmentProfile](../resources/appleuserinitiatedenrollmentprofile.md) collection|Apple user initiated enrollment profiles|
|auditEvents|[auditEvent](../resources/auditevent.md) collection|The Audit Events|
|autopilotEvents|[deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) collection|The list of autopilot events for the tenant.|
|cartToClassAssociations|[cartToClassAssociation](../resources/carttoclassassociation.md) collection|The Cart To Class Associations.|
|categories|[deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) collection|The available categories|
|complianceManagementPartners|[complianceManagementPartner](../resources/compliancemanagementpartner.md) collection|The list of Compliance Management Partners configured by the tenant.|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md)|The Exchange on premises conditional access settings. On premises conditional access will require devices to be both enrolled and compliant for mail access|
|dataSharingConsents|[dataSharingConsent](../resources/datasharingconsent.md) collection|Data sharing consents.|
|depOnboardingSettings|[depOnboardingSetting](../resources/deponboardingsetting.md) collection|This collections of multiple DEP tokens per-tenant.|
|derivedCredentials|[deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) collection|Collection of Derived credential settings associated with account.|
|detectedApps|[detectedApp](../resources/detectedapp.md) collection|The list of detected apps associated with a device.|
|deviceCategories|[deviceCategory](../resources/devicecategory.md) collection|The list of device categories with the tenant.|
|deviceCompliancePolicies|[deviceCompliancePolicy](../resources/devicecompliancepolicy.md) collection|The device compliance policies.|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/devicecompliancepolicydevicestatesummary.md)|The device compliance state summary for this account.|
|deviceCompliancePolicySettingStateSummaries|[deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md) collection|The summary states of compliance policy settings for this account.|
|deviceConfigurationConflictSummary|[deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md) collection|Summary of policies in conflict state for this account.|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/deviceconfigurationdevicestatesummary.md)|The device configuration device state summary for this account.|
|deviceConfigurationRestrictedAppsViolations|[restrictedAppsViolation](../resources/restrictedappsviolation.md) collection|Restricted apps violations for this account.|
|deviceConfigurations|[deviceConfiguration](../resources/deviceconfiguration.md) collection|The device configurations.|
|deviceConfigurationsAllManagedDeviceCertificateStates|[managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md) collection|Summary of all certificates for all devices.|
|deviceConfigurationUserStateSummaries|[deviceConfigurationUserStateSummary](../resources/deviceconfigurationuserstatesummary.md)|The device configuration user state summary for this account.|
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md) collection|The list of device enrollment configurations|
|deviceHealthScripts|[deviceHealthScript](../resources/devicehealthscript.md) collection|The list of device health scripts associated with the tenant.|
|deviceManagementPartners|[deviceManagementPartner](../resources/devicemanagementpartner.md) collection|The list of Device Management Partners configured by the tenant.|
|deviceManagementScripts|[deviceManagementScript](../resources/devicemanagementscript.md) collection|The list of device management scripts associated with the tenant.|
|deviceShellScripts|[deviceShellScript](../resources/deviceshellscript.md) collection|The list of device shell scripts associated with the tenant.|
|domainJoinConnectors|[deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md) collection|A list of connector objects.|
|embeddedSIMActivationCodePools|[embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md) collection|The embedded SIM activation code pools created by this account.|
|exchangeConnectors|[deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) collection|The list of Exchange Connectors configured by the tenant.|
|exchangeOnPremisesPolicies|[deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md) collection|The list of Exchange On Premisis policies configured by the tenant.|
|exchangeOnPremisesPolicy|[deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md)|The policy which controls mobile device access to Exchange On Premises|
|groupPolicyCategories|[groupPolicyCategory](../resources/grouppolicycategory.md) collection|The available group policy categories for this account.|
|groupPolicyConfigurations|[groupPolicyConfiguration](../resources/grouppolicyconfiguration.md) collection|The group policy configurations created by this account.|
|groupPolicyDefinitionFiles|[groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) collection|The available group policy definition files for this account.|
|groupPolicyDefinitions|[groupPolicyDefinition](../resources/grouppolicydefinition.md) collection|The available group policy definitions for this account.|
|groupPolicyMigrationReports|[groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) collection|A list of Group Policy migration reports.|
|groupPolicyObjectFiles|[groupPolicyObjectFile](../resources/grouppolicyobjectfile.md) collection|A list of Group Policy Object files uploaded.|
|groupPolicyUploadedDefinitionFiles|[groupPolicyUploadedDefinitionFile](../resources/grouppolicyuploadeddefinitionfile.md) collection|The available group policy uploaded definition files for this account.|
|importedDeviceIdentities|[importedDeviceIdentity](../resources/importeddeviceidentity.md) collection|The imported device identities.|
|importedWindowsAutopilotDeviceIdentities|[importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md) collection|Collection of imported Windows autopilot devices.|
|intents|[deviceManagementIntent](../resources/devicemanagementintent.md) collection|The device management intents|
|intuneBrandingProfiles|[intuneBrandingProfile](../resources/intunebrandingprofile.md) collection|Intune branding profiles targeted to AAD groups|
|iosUpdateStatuses|[iosUpdateDeviceStatus](../resources/iosupdatedevicestatus.md) collection|The IOS software update installation statuses for this account.|
|managedDeviceEncryptionStates|[managedDeviceEncryptionState](../resources/manageddeviceencryptionstate.md) collection|Encryption report for devices in this account|
|managedDeviceOverview|[managedDeviceOverview](../resources/manageddeviceoverview.md)|Device overview|
|managedDevices|[managedDevice](../resources/manageddevice.md) collection|The list of managed devices.|
|managementConditions|[managementCondition](../resources/managementcondition.md) collection|The management conditions associated with device management of the company.|
|managementConditionStatements|[managementConditionStatement](../resources/managementconditionstatement.md) collection|The management condition statements associated with device management of the company.|
|mobileAppTroubleshootingEvents|[mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md) collection|The collection property of MobileAppTroubleshootingEvent.|
|mobileThreatDefenseConnectors|[mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) collection|The list of Mobile threat Defense connectors configured by the tenant.|
|ndesConnectors|[ndesConnector](../resources/ndesconnector.md) collection|The collection of Ndes connectors for this account.|
|notificationMessageTemplates|[notificationMessageTemplate](../resources/notificationmessagetemplate.md) collection|The Notification Message Templates.|
|remoteActionAudits|[remoteActionAudit](../resources/remoteactionaudit.md) collection|The list of device remote action audits with the tenant.|
|remoteAssistancePartners|[remoteAssistancePartner](../resources/remoteassistancepartner.md) collection|The remote assist partners.|
|reports|[deviceManagementReports](../resources/devicemanagementreports.md)|Reports singleton|
|resourceOperations|[resourceOperation](../resources/resourceoperation.md) collection|The Resource Operations.|
|roleAssignments|[deviceAndAppManagementRoleAssignment](../resources/deviceandappmanagementroleassignment.md) collection|The Role Assignments.|
|roleDefinitions|[roleDefinition](../resources/roledefinition.md) collection|The Role Definitions.|
|roleScopeTags|[roleScopeTag](../resources/rolescopetag.md) collection|The Role Scope Tags.|
|settingDefinitions|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) collection|The device management intent setting definitions|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md)|The software update status summary.|
|telecomExpenseManagementPartners|[telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) collection|The telecom expense management partners.|
|templates|[deviceManagementTemplate](../resources/devicemanagementtemplate.md) collection|The available templates|
|termsAndConditions|[termsAndConditions](../resources/termsandconditions.md) collection|The terms and conditions associated with device management of the company.|
|troubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md) collection|The list of troubleshooting events for the tenant.|
|userExperienceAnalyticsBaselines|[userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md) collection|User experience analytics baselines|
|userExperienceAnalyticsCategories|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) collection|User experience analytics categories|
|userExperienceAnalyticsDevicePerformance|[userExperienceAnalyticsDevicePerformance](../resources/userexperienceanalyticsdeviceperformance.md) collection|User experience analytics device performance|
|userExperienceAnalyticsDeviceStartupHistory|[userExperienceAnalyticsDeviceStartupHistory](../resources/userexperienceanalyticsdevicestartuphistory.md) collection|User experience analytics device Startup History|
|userExperienceAnalyticsDeviceStartupProcesses|[userExperienceAnalyticsDeviceStartupProcess](../resources/userexperienceanalyticsdevicestartupprocess.md) collection|User experience analytics device Startup Processes|
|userExperienceAnalyticsDeviceStartupProcessPerformance|[userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/userexperienceanalyticsdevicestartupprocessperformance.md) collection|User experience analytics device Startup Process Performance|
|userExperienceAnalyticsOverview|[userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md)|User experience analytics overview|
|userExperienceAnalyticsRegressionSummary|[userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md)|User experience analytics regression summary|
|userExperienceAnalyticsScoreHistory|[userExperienceAnalyticsScoreHistory](../resources/userexperienceanalyticsscorehistory.md) collection|User experience analytics device Startup Score History|
|userPfxCertificates|[userPFXCertificate](../resources/userpfxcertificate.md) collection|Collection of PFX certificates associated with a user.|
|windowsAutopilotDeploymentProfiles|[windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md) collection|Windows auto pilot deployment profiles|
|windowsAutopilotDeviceIdentities|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) collection|The Windows autopilot device identities contained collection.|
|windowsAutopilotSettings|[windowsAutopilotSettings](../resources/windowsautopilotsettings.md)|The Windows autopilot account settings.|
|windowsFeatureUpdateProfiles|[windowsFeatureUpdateProfile](../resources/windowsfeatureupdateprofile.md) collection|A collection of windows feature update profiles|
|windowsInformationProtectionAppLearningSummaries|[windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md) collection|The windows information protection app learning summaries.|
|windowsInformationProtectionNetworkLearningSummaries|[windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md) collection|The windows information protection network learning summaries.|
|windowsMalwareInformation|[windowsMalwareInformation](../resources/windowsmalwareinformation.md) collection|The list of affected malware in the tenant.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 1024,
    "isScheduledActionEnabled": true,
    "secureByDefault": true,
    "enhancedJailBreak": true,
    "deviceInactivityBeforeRetirementInDay": 1024,
    "derivedCredentialProvider": "String",
    "derivedCredentialUrl": "String",
    "androidDeviceAdministratorEnrollmentEnabled": true,
    "ignoreDevicesForUnsupportedSettingsEnabled": true
  },
  "maximumDepTokens": 1024,
  "intuneAccountId": "Guid",
  "lastReportAggregationDateTime": "String (timestamp)",
  "deviceComplianceReportSummarizationDateTime": "String (timestamp)",
  "legacyPcManangementEnabled": true,
  "intuneBrand": {
    "@odata.type": "microsoft.graph.intuneBrand",
    "themeColor": {
      "@odata.type": "microsoft.graph.rgbColor",
      "r": 1024,
      "g": 1024,
      "b": 1024
    },
    "showLogo": true,
    "lightBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "String",
      "value": "binary"
    },
    "darkBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent"
    },
    "showNameNextToLogo": true,
    "landingPageCustomizedImage": {
      "@odata.type": "microsoft.graph.mimeContent"
    },
    "showDisplayNameNextToLogo": true,
    "roleScopeTagIds": [
      "String"
    ],
    "contactITName": "String",
    "contactITPhoneNumber": "String",
    "contactITEmailAddress": "String",
    "contactITNotes": "String",
    "onlineSupportSiteUrl": "String",
    "onlineSupportSiteName": "String",
    "privacyUrl": "String",
    "customPrivacyMessage": "String",
    "isRemoveDeviceDisabled": true,
    "isFactoryResetDisabled": true,
    "companyPortalBlockedActions": [
      {
        "@odata.type": "microsoft.graph.companyPortalBlockedAction",
        "platform": "String",
        "ownerType": "String",
        "action": "String"
      }
    ],
    "showAzureADEnterpriseApps": true,
    "showOfficeWebApps": true,
    "sendDeviceOwnershipChangePushNotification": true,
    "enrollmentAvailability": "String"
  },
  "subscriptionState": "String",
  "subscriptions": "String",
  "managedDeviceCleanupSettings": {
    "@odata.type": "microsoft.graph.managedDeviceCleanupSettings",
    "deviceInactivityBeforeRetirementInDays": "String"
  },
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "String",
    "shareUserExperienceAnalyticsData": "String"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 1024,
    "inactiveThreatAgentDeviceCount": 1024,
    "unknownStateThreatAgentDeviceCount": 1024,
    "pendingSignatureUpdateDeviceCount": 1024,
    "cleanDeviceCount": 1024,
    "pendingFullScanDeviceCount": 1024,
    "pendingRestartDeviceCount": 1024,
    "pendingManualStepsDeviceCount": 1024,
    "pendingOfflineScanDeviceCount": 1024,
    "criticalFailuresDeviceCount": 1024
  },
  "windowsMalwareOverview": {
    "@odata.type": "microsoft.graph.windowsMalwareOverview",
    "malwareDetectedDeviceCount": 1024,
    "malwareStateSummary": [
      {
        "@odata.type": "microsoft.graph.windowsMalwareStateCount",
        "state": "String",
        "deviceCount": 1024,
        "lastUpdateDateTime": "String (timestamp)"
      }
    ],
    "malwareExecutionStateSummary": [
      {
        "@odata.type": "microsoft.graph.windowsMalwareExecutionStateCount",
        "executionState": "String"
      }
    ],
    "malwareCategorySummary": [
      {
        "@odata.type": "microsoft.graph.windowsMalwareCategoryCount"
      }
    ],
    "malwareNameSummary": [
      {
        "@odata.type": "microsoft.graph.windowsMalwareNameCount",
        "malwareIdentifier": "String",
        "name": "String"
      }
    ],
    "osVersionsSummary": [
      {
        "@odata.type": "microsoft.graph.osVersionCount",
        "osVersion": "String"
      }
    ]
  },
  "accountMoveCompletionDateTime": "String (timestamp)"
}
```

