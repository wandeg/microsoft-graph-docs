---
title: "deviceManagement resource type"
description: "Singleton entity that acts as a container for Android for Work settings functionality under device management."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceManagement resource type

Singleton entity that acts as a container for Android for Work settings functionality under device management.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagement](../api/intune-devices-devicemanagement-get.md)|[deviceManagement](../resources/intune-devices-deviceManagement.md)|Read properties and relationships of the [deviceManagement](../resources/devicemanagement.md) object.|
|[Update deviceManagement](../api/intune-devices-devicemanagement-update.md)|[deviceManagement](../resources/intune-devices-deviceManagement.md)|Update the properties of a [deviceManagement](../resources/devicemanagement.md) object.|
|[enableLegacyPcManagement](../api/intune-devices-devicemanagement-enablelegacypcmanagement.md)|None||
|[enableAndroidDeviceAdministratorEnrollment](../api/intune-devices-devicemanagement-enableandroiddeviceadministratorenrollment.md)|None||
|[verifyWindowsEnrollmentAutoDiscovery](../api/intune-devices-devicemanagement-verifywindowsenrollmentautodiscovery.md)|Boolean||
|[sendCustomNotificationToCompanyPortal](../api/intune-devices-devicemanagement-sendcustomnotificationtocompanyportal.md)|None||
|[getEffectivePermissions](../api/intune-devices-devicemanagement-geteffectivepermissions.md)|String collection||
|[getEffectivePermissions](../api/intune-devices-devicemanagement-geteffectivepermissions.md)|[rolePermission](../resources/rolePermission.md) collection||
|[getRoleScopeTagsByResource](../api/intune-devices-devicemanagement-getrolescopetagsbyresource.md)|[roleScopeTag](../resources/roleScopeTag.md) collection||
|[getRoleScopeTagsByIds](../api/intune-devices-devicemanagement-getrolescopetagsbyids.md)|[roleScopeTag](../resources/roleScopeTag.md) collection||
|[getAssignedRoleDetails](../api/intune-devices-devicemanagement-getassignedroledetails.md)|[deviceAndAppManagementAssignedRoleDetails](../resources/deviceAndAppManagementAssignedRoleDetails.md)||
|[scopedForResource](../api/intune-devices-devicemanagement-scopedforresource.md)|Boolean||
|[List auditEvents](../api/intune-devices-devicemanagement-list-auditevents.md)|[auditEvent](../resources/auditEvent.md) collection|Get the auditEvents from the auditEvents navigation property.|
|[Add auditEvents](../api/intune-devices-devicemanagement-post-auditevents.md)|[auditEvent](../resources/auditEvent.md)|Add auditEvents by posting to the auditEvents collection.|
|[Get androidForWorkSettings](../api/androidforworksettings-get.md)|[androidForWorkSettings](../resources/androidForWorkSettings.md)|Read properties and relationships of the [androidForWorkSettings](../resources/androidforworksettings.md) object.|
|[List androidForWorkAppConfigurationSchemas](../api/intune-devices-devicemanagement-list-androidforworkappconfigurationschemas.md)|[androidForWorkAppConfigurationSchema](../resources/androidForWorkAppConfigurationSchema.md) collection|Get the androidForWorkAppConfigurationSchemas from the androidForWorkAppConfigurationSchemas navigation property.|
|[Add androidForWorkAppConfigurationSchemas](../api/intune-devices-devicemanagement-post-androidforworkappconfigurationschemas.md)|[androidForWorkAppConfigurationSchema](../resources/androidForWorkAppConfigurationSchema.md)|Add androidForWorkAppConfigurationSchemas by posting to the androidForWorkAppConfigurationSchemas collection.|
|[List androidForWorkEnrollmentProfiles](../api/intune-devices-devicemanagement-list-androidforworkenrollmentprofiles.md)|[androidForWorkEnrollmentProfile](../resources/androidForWorkEnrollmentProfile.md) collection|Get the androidForWorkEnrollmentProfiles from the androidForWorkEnrollmentProfiles navigation property.|
|[Add androidForWorkEnrollmentProfiles](../api/intune-devices-devicemanagement-post-androidforworkenrollmentprofiles.md)|[androidForWorkEnrollmentProfile](../resources/androidForWorkEnrollmentProfile.md)|Add androidForWorkEnrollmentProfiles by posting to the androidForWorkEnrollmentProfiles collection.|
|[Get androidManagedStoreAccountEnterpriseSettings](../api/androidmanagedstoreaccountenterprisesettings-get.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/androidManagedStoreAccountEnterpriseSettings.md)|Read properties and relationships of the [androidManagedStoreAccountEnterpriseSettings](../resources/androidmanagedstoreaccountenterprisesettings.md) object.|
|[List androidManagedStoreAppConfigurationSchemas](../api/intune-devices-devicemanagement-list-androidmanagedstoreappconfigurationschemas.md)|[androidManagedStoreAppConfigurationSchema](../resources/androidManagedStoreAppConfigurationSchema.md) collection|Get the androidManagedStoreAppConfigurationSchemas from the androidManagedStoreAppConfigurationSchemas navigation property.|
|[Add androidManagedStoreAppConfigurationSchemas](../api/intune-devices-devicemanagement-post-androidmanagedstoreappconfigurationschemas.md)|[androidManagedStoreAppConfigurationSchema](../resources/androidManagedStoreAppConfigurationSchema.md)|Add androidManagedStoreAppConfigurationSchemas by posting to the androidManagedStoreAppConfigurationSchemas collection.|
|[List androidDeviceOwnerEnrollmentProfiles](../api/intune-devices-devicemanagement-list-androiddeviceownerenrollmentprofiles.md)|[androidDeviceOwnerEnrollmentProfile](../resources/androidDeviceOwnerEnrollmentProfile.md) collection|Get the androidDeviceOwnerEnrollmentProfiles from the androidDeviceOwnerEnrollmentProfiles navigation property.|
|[Add androidDeviceOwnerEnrollmentProfiles](../api/intune-devices-devicemanagement-post-androiddeviceownerenrollmentprofiles.md)|[androidDeviceOwnerEnrollmentProfile](../resources/androidDeviceOwnerEnrollmentProfile.md)|Add androidDeviceOwnerEnrollmentProfiles by posting to the androidDeviceOwnerEnrollmentProfiles collection.|
|[List termsAndConditions](../api/intune-devices-devicemanagement-list-termsandconditions.md)|[termsAndConditions](../resources/termsAndConditions.md) collection|Get the termsAndConditionses from the termsAndConditions navigation property.|
|[Add termsAndConditions](../api/intune-devices-devicemanagement-post-termsandconditions.md)|[termsAndConditions](../resources/termsAndConditions.md)|Add termsAndConditions by posting to the termsAndConditions collection.|
|[List userPfxCertificates](../api/intune-devices-devicemanagement-list-userpfxcertificates.md)|[userPFXCertificate](../resources/userPFXCertificate.md) collection|Get the userPFXCertificates from the userPfxCertificates navigation property.|
|[Add userPfxCertificates](../api/intune-devices-devicemanagement-post-userpfxcertificates.md)|[userPFXCertificate](../resources/userPFXCertificate.md)|Add userPfxCertificates by posting to the userPfxCertificates collection.|
|[List deviceConfigurations](../api/intune-devices-devicemanagement-list-deviceconfigurations.md)|[deviceConfiguration](../resources/deviceConfiguration.md) collection|Get the deviceConfigurations from the deviceConfigurations navigation property.|
|[Add deviceConfigurations](../api/intune-devices-devicemanagement-post-deviceconfigurations.md)|[deviceConfiguration](../resources/deviceConfiguration.md)|Add deviceConfigurations by posting to the deviceConfigurations collection.|
|[List deviceCompliancePolicies](../api/intune-devices-devicemanagement-list-devicecompliancepolicies.md)|[deviceCompliancePolicy](../resources/deviceCompliancePolicy.md) collection|Get the deviceCompliancePolicies from the deviceCompliancePolicies navigation property.|
|[Add deviceCompliancePolicies](../api/intune-devices-devicemanagement-post-devicecompliancepolicies.md)|[deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|Add deviceCompliancePolicies by posting to the deviceCompliancePolicies collection.|
|[Get softwareUpdateStatusSummary](../api/softwareupdatestatussummary-get.md)|[softwareUpdateStatusSummary](../resources/softwareUpdateStatusSummary.md)|Read properties and relationships of the [softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md) object.|
|[Get deviceCompliancePolicyDeviceStateSummary](../api/devicecompliancepolicydevicestatesummary-get.md)|[deviceCompliancePolicyDeviceStateSummary](../resources/deviceCompliancePolicyDeviceStateSummary.md)|Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/devicecompliancepolicydevicestatesummary.md) object.|
|[List deviceCompliancePolicySettingStateSummaries](../api/intune-devices-devicemanagement-list-devicecompliancepolicysettingstatesummaries.md)|[deviceCompliancePolicySettingStateSummary](../resources/deviceCompliancePolicySettingStateSummary.md) collection|Get the deviceCompliancePolicySettingStateSummaries from the deviceCompliancePolicySettingStateSummaries navigation property.|
|[Add deviceCompliancePolicySettingStateSummaries](../api/intune-devices-devicemanagement-post-devicecompliancepolicysettingstatesummaries.md)|[deviceCompliancePolicySettingStateSummary](../resources/deviceCompliancePolicySettingStateSummary.md)|Add deviceCompliancePolicySettingStateSummaries by posting to the deviceCompliancePolicySettingStateSummaries collection.|
|[Get advancedThreatProtectionOnboardingStateSummary](../api/advancedthreatprotectiononboardingstatesummary-get.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/advancedThreatProtectionOnboardingStateSummary.md)|Read properties and relationships of the [advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md) object.|
|[Get deviceConfigurationDeviceStateSummary](../api/deviceconfigurationdevicestatesummary-get.md)|[deviceConfigurationDeviceStateSummary](../resources/deviceConfigurationDeviceStateSummary.md)|Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/deviceconfigurationdevicestatesummary.md) object.|
|[Get deviceConfigurationUserStateSummary](../api/deviceconfigurationuserstatesummary-get.md)|[deviceConfigurationUserStateSummary](../resources/deviceConfigurationUserStateSummary.md)|Read properties and relationships of the [deviceConfigurationUserStateSummary](../resources/deviceconfigurationuserstatesummary.md) object.|
|[List cartToClassAssociations](../api/intune-devices-devicemanagement-list-carttoclassassociations.md)|[cartToClassAssociation](../resources/cartToClassAssociation.md) collection|Get the cartToClassAssociations from the cartToClassAssociations navigation property.|
|[Add cartToClassAssociations](../api/intune-devices-devicemanagement-post-carttoclassassociations.md)|[cartToClassAssociation](../resources/cartToClassAssociation.md)|Add cartToClassAssociations by posting to the cartToClassAssociations collection.|
|[List iosUpdateStatuses](../api/intune-devices-devicemanagement-list-iosupdatestatuses.md)|[iosUpdateDeviceStatus](../resources/iosUpdateDeviceStatus.md) collection|Get the iosUpdateDeviceStatuses from the iosUpdateStatuses navigation property.|
|[Add iosUpdateStatuses](../api/intune-devices-devicemanagement-post-iosupdatestatuses.md)|[iosUpdateDeviceStatus](../resources/iosUpdateDeviceStatus.md)|Add iosUpdateStatuses by posting to the iosUpdateStatuses collection.|
|[List ndesConnectors](../api/intune-devices-devicemanagement-list-ndesconnectors.md)|[ndesConnector](../resources/ndesConnector.md) collection|Get the ndesConnectors from the ndesConnectors navigation property.|
|[Add ndesConnectors](../api/intune-devices-devicemanagement-post-ndesconnectors.md)|[ndesConnector](../resources/ndesConnector.md)|Add ndesConnectors by posting to the ndesConnectors collection.|
|[List deviceConfigurationRestrictedAppsViolations](../api/intune-devices-devicemanagement-list-deviceconfigurationrestrictedappsviolations.md)|[restrictedAppsViolation](../resources/restrictedAppsViolation.md) collection|Get the restrictedAppsViolations from the deviceConfigurationRestrictedAppsViolations navigation property.|
|[Add deviceConfigurationRestrictedAppsViolations](../api/intune-devices-devicemanagement-post-deviceconfigurationrestrictedappsviolations.md)|[restrictedAppsViolation](../resources/restrictedAppsViolation.md)|Add deviceConfigurationRestrictedAppsViolations by posting to the deviceConfigurationRestrictedAppsViolations collection.|
|[List managedDeviceEncryptionStates](../api/intune-devices-devicemanagement-list-manageddeviceencryptionstates.md)|[managedDeviceEncryptionState](../resources/managedDeviceEncryptionState.md) collection|Get the managedDeviceEncryptionStates from the managedDeviceEncryptionStates navigation property.|
|[Add managedDeviceEncryptionStates](../api/intune-devices-devicemanagement-post-manageddeviceencryptionstates.md)|[managedDeviceEncryptionState](../resources/managedDeviceEncryptionState.md)|Add managedDeviceEncryptionStates by posting to the managedDeviceEncryptionStates collection.|
|[List deviceConfigurationConflictSummary](../api/intune-devices-devicemanagement-list-deviceconfigurationconflictsummary.md)|[deviceConfigurationConflictSummary](../resources/deviceConfigurationConflictSummary.md) collection|Get the deviceConfigurationConflictSummaries from the deviceConfigurationConflictSummary navigation property.|
|[Add deviceConfigurationConflictSummary](../api/intune-devices-devicemanagement-post-deviceconfigurationconflictsummary.md)|[deviceConfigurationConflictSummary](../resources/deviceConfigurationConflictSummary.md)|Add deviceConfigurationConflictSummary by posting to the deviceConfigurationConflictSummary collection.|
|[List deviceConfigurationsAllManagedDeviceCertificateStates](../api/intune-devices-devicemanagement-list-deviceconfigurationsallmanageddevicecertificatestates.md)|[managedAllDeviceCertificateState](../resources/managedAllDeviceCertificateState.md) collection|Get the managedAllDeviceCertificateStates from the deviceConfigurationsAllManagedDeviceCertificateStates navigation property.|
|[Add deviceConfigurationsAllManagedDeviceCertificateStates](../api/intune-devices-devicemanagement-post-deviceconfigurationsallmanageddevicecertificatestates.md)|[managedAllDeviceCertificateState](../resources/managedAllDeviceCertificateState.md)|Add deviceConfigurationsAllManagedDeviceCertificateStates by posting to the deviceConfigurationsAllManagedDeviceCertificateStates collection.|
|[List deviceCategories](../api/intune-devices-devicemanagement-list-devicecategories.md)|[deviceCategory](../resources/deviceCategory.md) collection|Get the deviceCategories from the deviceCategories navigation property.|
|[Add deviceCategories](../api/intune-devices-devicemanagement-post-devicecategories.md)|[deviceCategory](../resources/deviceCategory.md)|Add deviceCategories by posting to the deviceCategories collection.|
|[List exchangeConnectors](../api/intune-devices-devicemanagement-list-exchangeconnectors.md)|[deviceManagementExchangeConnector](../resources/deviceManagementExchangeConnector.md) collection|Get the deviceManagementExchangeConnectors from the exchangeConnectors navigation property.|
|[Add exchangeConnectors](../api/intune-devices-devicemanagement-post-exchangeconnectors.md)|[deviceManagementExchangeConnector](../resources/deviceManagementExchangeConnector.md)|Add exchangeConnectors by posting to the exchangeConnectors collection.|
|[List deviceEnrollmentConfigurations](../api/intune-devices-devicemanagement-list-deviceenrollmentconfigurations.md)|[deviceEnrollmentConfiguration](../resources/deviceEnrollmentConfiguration.md) collection|Get the deviceEnrollmentConfigurations from the deviceEnrollmentConfigurations navigation property.|
|[Add deviceEnrollmentConfigurations](../api/intune-devices-devicemanagement-post-deviceenrollmentconfigurations.md)|[deviceEnrollmentConfiguration](../resources/deviceEnrollmentConfiguration.md)|Add deviceEnrollmentConfigurations by posting to the deviceEnrollmentConfigurations collection.|
|[Get deviceManagementExchangeOnPremisesPolicy](../api/devicemanagementexchangeonpremisespolicy-get.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/deviceManagementExchangeOnPremisesPolicy.md)|Read properties and relationships of the [deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md) object.|
|[List exchangeOnPremisesPolicies](../api/intune-devices-devicemanagement-list-exchangeonpremisespolicies.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/deviceManagementExchangeOnPremisesPolicy.md) collection|Get the deviceManagementExchangeOnPremisesPolicies from the exchangeOnPremisesPolicies navigation property.|
|[Add exchangeOnPremisesPolicies](../api/intune-devices-devicemanagement-post-exchangeonpremisespolicies.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/deviceManagementExchangeOnPremisesPolicy.md)|Add exchangeOnPremisesPolicies by posting to the exchangeOnPremisesPolicies collection.|
|[Get onPremisesConditionalAccessSettings](../api/onpremisesconditionalaccesssettings-get.md)|[onPremisesConditionalAccessSettings](../resources/onPremisesConditionalAccessSettings.md)|Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.|
|[List mobileThreatDefenseConnectors](../api/intune-devices-devicemanagement-list-mobilethreatdefenseconnectors.md)|[mobileThreatDefenseConnector](../resources/mobileThreatDefenseConnector.md) collection|Get the mobileThreatDefenseConnectors from the mobileThreatDefenseConnectors navigation property.|
|[Add mobileThreatDefenseConnectors](../api/intune-devices-devicemanagement-post-mobilethreatdefenseconnectors.md)|[mobileThreatDefenseConnector](../resources/mobileThreatDefenseConnector.md)|Add mobileThreatDefenseConnectors by posting to the mobileThreatDefenseConnectors collection.|
|[List deviceManagementPartners](../api/intune-devices-devicemanagement-list-devicemanagementpartners.md)|[deviceManagementPartner](../resources/deviceManagementPartner.md) collection|Get the deviceManagementPartners from the deviceManagementPartners navigation property.|
|[Add deviceManagementPartners](../api/intune-devices-devicemanagement-post-devicemanagementpartners.md)|[deviceManagementPartner](../resources/deviceManagementPartner.md)|Add deviceManagementPartners by posting to the deviceManagementPartners collection.|
|[List complianceManagementPartners](../api/intune-devices-devicemanagement-list-compliancemanagementpartners.md)|[complianceManagementPartner](../resources/complianceManagementPartner.md) collection|Get the complianceManagementPartners from the complianceManagementPartners navigation property.|
|[Add complianceManagementPartners](../api/intune-devices-devicemanagement-post-compliancemanagementpartners.md)|[complianceManagementPartner](../resources/complianceManagementPartner.md)|Add complianceManagementPartners by posting to the complianceManagementPartners collection.|
|[List intents](../api/intune-devices-devicemanagement-list-intents.md)|[deviceManagementIntent](../resources/deviceManagementIntent.md) collection|Get the deviceManagementIntents from the intents navigation property.|
|[Add intents](../api/intune-devices-devicemanagement-post-intents.md)|[deviceManagementIntent](../resources/deviceManagementIntent.md)|Add intents by posting to the intents collection.|
|[List settingDefinitions](../api/intune-devices-devicemanagement-list-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/deviceManagementSettingDefinition.md) collection|Get the deviceManagementSettingDefinitions from the settingDefinitions navigation property.|
|[Add settingDefinitions](../api/intune-devices-devicemanagement-post-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/deviceManagementSettingDefinition.md)|Add settingDefinitions by posting to the settingDefinitions collection.|
|[List templates](../api/intune-devices-devicemanagement-list-templates.md)|[deviceManagementTemplate](../resources/deviceManagementTemplate.md) collection|Get the deviceManagementTemplates from the templates navigation property.|
|[Add templates](../api/intune-devices-devicemanagement-post-templates.md)|[deviceManagementTemplate](../resources/deviceManagementTemplate.md)|Add templates by posting to the templates collection.|
|[List categories](../api/intune-devices-devicemanagement-list-categories.md)|[deviceManagementSettingCategory](../resources/deviceManagementSettingCategory.md) collection|Get the deviceManagementSettingCategories from the categories navigation property.|
|[Add categories](../api/intune-devices-devicemanagement-post-categories.md)|[deviceManagementSettingCategory](../resources/deviceManagementSettingCategory.md)|Add categories by posting to the categories collection.|
|[List remoteActionAudits](../api/intune-devices-devicemanagement-list-remoteactionaudits.md)|[remoteActionAudit](../resources/intune-devices-remoteActionAudit.md) collection|Get the remoteActionAudits from the remoteActionAudits navigation property.|
|[Add remoteActionAudits](../api/intune-devices-devicemanagement-post-remoteactionaudits.md)|[remoteActionAudit](../resources/intune-devices-remoteActionAudit.md)|Add remoteActionAudits by posting to the remoteActionAudits collection.|
|[Get applePushNotificationCertificate](../api/intune-devices-applepushnotificationcertificate-get.md)|[applePushNotificationCertificate](../resources/intune-devices-applePushNotificationCertificate.md)|Read properties and relationships of the [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object.|
|[List deviceManagementScripts](../api/intune-devices-devicemanagement-list-devicemanagementscripts.md)|[deviceManagementScript](../resources/intune-devices-deviceManagementScript.md) collection|Get the deviceManagementScripts from the deviceManagementScripts navigation property.|
|[Add deviceManagementScripts](../api/intune-devices-devicemanagement-post-devicemanagementscripts.md)|[deviceManagementScript](../resources/intune-devices-deviceManagementScript.md)|Add deviceManagementScripts by posting to the deviceManagementScripts collection.|
|[List deviceShellScripts](../api/intune-devices-devicemanagement-list-deviceshellscripts.md)|[deviceShellScript](../resources/intune-devices-deviceShellScript.md) collection|Get the deviceShellScripts from the deviceShellScripts navigation property.|
|[Add deviceShellScripts](../api/intune-devices-devicemanagement-post-deviceshellscripts.md)|[deviceShellScript](../resources/intune-devices-deviceShellScript.md)|Add deviceShellScripts by posting to the deviceShellScripts collection.|
|[List deviceHealthScripts](../api/intune-devices-devicemanagement-list-devicehealthscripts.md)|[deviceHealthScript](../resources/intune-devices-deviceHealthScript.md) collection|Get the deviceHealthScripts from the deviceHealthScripts navigation property.|
|[Add deviceHealthScripts](../api/intune-devices-devicemanagement-post-devicehealthscripts.md)|[deviceHealthScript](../resources/intune-devices-deviceHealthScript.md)|Add deviceHealthScripts by posting to the deviceHealthScripts collection.|
|[Get managedDeviceOverview](../api/intune-devices-manageddeviceoverview-get.md)|[managedDeviceOverview](../resources/intune-devices-managedDeviceOverview.md)|Read properties and relationships of the [managedDeviceOverview](../resources/manageddeviceoverview.md) object.|
|[List detectedApps](../api/intune-devices-devicemanagement-list-detectedapps.md)|[detectedApp](../resources/intune-devices-detectedApp.md) collection|Get the detectedApps from the detectedApps navigation property.|
|[Add detectedApps](../api/intune-devices-devicemanagement-post-detectedapps.md)|[detectedApp](../resources/intune-devices-detectedApp.md)|Add detectedApps by posting to the detectedApps collection.|
|[List managedDevices](../api/intune-devices-devicemanagement-list-manageddevices.md)|[managedDevice](../resources/intune-devices-managedDevice.md) collection|Get the managedDevices from the managedDevices navigation property.|
|[Add managedDevices](../api/intune-devices-devicemanagement-post-manageddevices.md)|[managedDevice](../resources/intune-devices-managedDevice.md)|Add managedDevices by posting to the managedDevices collection.|
|[List windowsMalwareInformation](../api/intune-devices-devicemanagement-list-windowsmalwareinformation.md)|[windowsMalwareInformation](../resources/intune-devices-windowsMalwareInformation.md) collection|Get the windowsMalwareInformations from the windowsMalwareInformation navigation property.|
|[Add windowsMalwareInformation](../api/intune-devices-devicemanagement-post-windowsmalwareinformation.md)|[windowsMalwareInformation](../resources/intune-devices-windowsMalwareInformation.md)|Add windowsMalwareInformation by posting to the windowsMalwareInformation collection.|
|[List dataSharingConsents](../api/intune-devices-devicemanagement-list-datasharingconsents.md)|[dataSharingConsent](../resources/intune-devices-dataSharingConsent.md) collection|Get the dataSharingConsents from the dataSharingConsents navigation property.|
|[Add dataSharingConsents](../api/intune-devices-devicemanagement-post-datasharingconsents.md)|[dataSharingConsent](../resources/intune-devices-dataSharingConsent.md)|Add dataSharingConsents by posting to the dataSharingConsents collection.|
|[List mobileAppTroubleshootingEvents](../api/intune-devices-devicemanagement-list-mobileapptroubleshootingevents.md)|[mobileAppTroubleshootingEvent](../resources/mobileAppTroubleshootingEvent.md) collection|Get the mobileAppTroubleshootingEvents from the mobileAppTroubleshootingEvents navigation property.|
|[Add mobileAppTroubleshootingEvents](../api/intune-devices-devicemanagement-post-mobileapptroubleshootingevents.md)|[mobileAppTroubleshootingEvent](../resources/mobileAppTroubleshootingEvent.md)|Add mobileAppTroubleshootingEvents by posting to the mobileAppTroubleshootingEvents collection.|
|[Get userExperienceAnalyticsOverview](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[userExperienceAnalyticsOverview](../resources/intune-devices-userExperienceAnalyticsOverview.md)|Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md) object.|
|[List userExperienceAnalyticsBaselines](../api/intune-devices-devicemanagement-list-userexperienceanalyticsbaselines.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userExperienceAnalyticsBaseline.md) collection|Get the userExperienceAnalyticsBaselines from the userExperienceAnalyticsBaselines navigation property.|
|[Add userExperienceAnalyticsBaselines](../api/intune-devices-devicemanagement-post-userexperienceanalyticsbaselines.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userExperienceAnalyticsBaseline.md)|Add userExperienceAnalyticsBaselines by posting to the userExperienceAnalyticsBaselines collection.|
|[List userExperienceAnalyticsCategories](../api/intune-devices-devicemanagement-list-userexperienceanalyticscategories.md)|[userExperienceAnalyticsCategory](../resources/intune-devices-userExperienceAnalyticsCategory.md) collection|Get the userExperienceAnalyticsCategories from the userExperienceAnalyticsCategories navigation property.|
|[Add userExperienceAnalyticsCategories](../api/intune-devices-devicemanagement-post-userexperienceanalyticscategories.md)|[userExperienceAnalyticsCategory](../resources/intune-devices-userExperienceAnalyticsCategory.md)|Add userExperienceAnalyticsCategories by posting to the userExperienceAnalyticsCategories collection.|
|[List userExperienceAnalyticsDevicePerformance](../api/intune-devices-devicemanagement-list-userexperienceanalyticsdeviceperformance.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userExperienceAnalyticsDevicePerformance.md) collection|Get the userExperienceAnalyticsDevicePerformances from the userExperienceAnalyticsDevicePerformance navigation property.|
|[Add userExperienceAnalyticsDevicePerformance](../api/intune-devices-devicemanagement-post-userexperienceanalyticsdeviceperformance.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userExperienceAnalyticsDevicePerformance.md)|Add userExperienceAnalyticsDevicePerformance by posting to the userExperienceAnalyticsDevicePerformance collection.|
|[Get userExperienceAnalyticsRegressionSummary](../api/intune-devices-userexperienceanalyticsregressionsummary-get.md)|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userExperienceAnalyticsRegressionSummary.md)|Read properties and relationships of the [userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md) object.|
|[List userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-devicemanagement-list-userexperienceanalyticsdevicestartuphistory.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userExperienceAnalyticsDeviceStartupHistory.md) collection|Get the userExperienceAnalyticsDeviceStartupHistories from the userExperienceAnalyticsDeviceStartupHistory navigation property.|
|[Add userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-devicemanagement-post-userexperienceanalyticsdevicestartuphistory.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userExperienceAnalyticsDeviceStartupHistory.md)|Add userExperienceAnalyticsDeviceStartupHistory by posting to the userExperienceAnalyticsDeviceStartupHistory collection.|
|[List derivedCredentials](../api/intune-devices-devicemanagement-list-derivedcredentials.md)|[deviceManagementDerivedCredentialSettings](../resources/deviceManagementDerivedCredentialSettings.md) collection|Get the deviceManagementDerivedCredentialSettingses from the derivedCredentials navigation property.|
|[Add derivedCredentials](../api/intune-devices-devicemanagement-post-derivedcredentials.md)|[deviceManagementDerivedCredentialSettings](../resources/deviceManagementDerivedCredentialSettings.md)|Add derivedCredentials by posting to the derivedCredentials collection.|
|[Get windowsAutopilotSettings](../api/windowsautopilotsettings-get.md)|[windowsAutopilotSettings](../resources/windowsAutopilotSettings.md)|Read properties and relationships of the [windowsAutopilotSettings](../resources/windowsautopilotsettings.md) object.|
|[List windowsAutopilotDeviceIdentities](../api/intune-devices-devicemanagement-list-windowsautopilotdeviceidentities.md)|[windowsAutopilotDeviceIdentity](../resources/windowsAutopilotDeviceIdentity.md) collection|Get the windowsAutopilotDeviceIdentities from the windowsAutopilotDeviceIdentities navigation property.|
|[Add windowsAutopilotDeviceIdentities](../api/intune-devices-devicemanagement-post-windowsautopilotdeviceidentities.md)|[windowsAutopilotDeviceIdentity](../resources/windowsAutopilotDeviceIdentity.md)|Add windowsAutopilotDeviceIdentities by posting to the windowsAutopilotDeviceIdentities collection.|
|[List windowsAutopilotDeploymentProfiles](../api/intune-devices-devicemanagement-list-windowsautopilotdeploymentprofiles.md)|[windowsAutopilotDeploymentProfile](../resources/windowsAutopilotDeploymentProfile.md) collection|Get the windowsAutopilotDeploymentProfiles from the windowsAutopilotDeploymentProfiles navigation property.|
|[Add windowsAutopilotDeploymentProfiles](../api/intune-devices-devicemanagement-post-windowsautopilotdeploymentprofiles.md)|[windowsAutopilotDeploymentProfile](../resources/windowsAutopilotDeploymentProfile.md)|Add windowsAutopilotDeploymentProfiles by posting to the windowsAutopilotDeploymentProfiles collection.|
|[List importedDeviceIdentities](../api/intune-devices-devicemanagement-list-importeddeviceidentities.md)|[importedDeviceIdentity](../resources/importedDeviceIdentity.md) collection|Get the importedDeviceIdentities from the importedDeviceIdentities navigation property.|
|[Add importedDeviceIdentities](../api/intune-devices-devicemanagement-post-importeddeviceidentities.md)|[importedDeviceIdentity](../resources/importedDeviceIdentity.md)|Add importedDeviceIdentities by posting to the importedDeviceIdentities collection.|
|[List depOnboardingSettings](../api/intune-devices-devicemanagement-list-deponboardingsettings.md)|[depOnboardingSetting](../resources/depOnboardingSetting.md) collection|Get the depOnboardingSettings from the depOnboardingSettings navigation property.|
|[Add depOnboardingSettings](../api/intune-devices-devicemanagement-post-deponboardingsettings.md)|[depOnboardingSetting](../resources/depOnboardingSetting.md)|Add depOnboardingSettings by posting to the depOnboardingSettings collection.|
|[List importedWindowsAutopilotDeviceIdentities](../api/intune-devices-devicemanagement-list-importedwindowsautopilotdeviceidentities.md)|[importedWindowsAutopilotDeviceIdentity](../resources/importedWindowsAutopilotDeviceIdentity.md) collection|Get the importedWindowsAutopilotDeviceIdentities from the importedWindowsAutopilotDeviceIdentities navigation property.|
|[Add importedWindowsAutopilotDeviceIdentities](../api/intune-devices-devicemanagement-post-importedwindowsautopilotdeviceidentities.md)|[importedWindowsAutopilotDeviceIdentity](../resources/importedWindowsAutopilotDeviceIdentity.md)|Add importedWindowsAutopilotDeviceIdentities by posting to the importedWindowsAutopilotDeviceIdentities collection.|
|[List appleUserInitiatedEnrollmentProfiles](../api/intune-devices-devicemanagement-list-appleuserinitiatedenrollmentprofiles.md)|[appleUserInitiatedEnrollmentProfile](../resources/appleUserInitiatedEnrollmentProfile.md) collection|Get the appleUserInitiatedEnrollmentProfiles from the appleUserInitiatedEnrollmentProfiles navigation property.|
|[Add appleUserInitiatedEnrollmentProfiles](../api/intune-devices-devicemanagement-post-appleuserinitiatedenrollmentprofiles.md)|[appleUserInitiatedEnrollmentProfile](../resources/appleUserInitiatedEnrollmentProfile.md)|Add appleUserInitiatedEnrollmentProfiles by posting to the appleUserInitiatedEnrollmentProfiles collection.|
|[List managementConditions](../api/intune-devices-devicemanagement-list-managementconditions.md)|[managementCondition](../resources/managementCondition.md) collection|Get the managementConditions from the managementConditions navigation property.|
|[Add managementConditions](../api/intune-devices-devicemanagement-post-managementconditions.md)|[managementCondition](../resources/managementCondition.md)|Add managementConditions by posting to the managementConditions collection.|
|[List managementConditionStatements](../api/intune-devices-devicemanagement-list-managementconditionstatements.md)|[managementConditionStatement](../resources/managementConditionStatement.md) collection|Get the managementConditionStatements from the managementConditionStatements navigation property.|
|[Add managementConditionStatements](../api/intune-devices-devicemanagement-post-managementconditionstatements.md)|[managementConditionStatement](../resources/managementConditionStatement.md)|Add managementConditionStatements by posting to the managementConditionStatements collection.|
|[List groupPolicyMigrationReports](../api/intune-devices-devicemanagement-list-grouppolicymigrationreports.md)|[groupPolicyMigrationReport](../resources/groupPolicyMigrationReport.md) collection|Get the groupPolicyMigrationReports from the groupPolicyMigrationReports navigation property.|
|[Add groupPolicyMigrationReports](../api/intune-devices-devicemanagement-post-grouppolicymigrationreports.md)|[groupPolicyMigrationReport](../resources/groupPolicyMigrationReport.md)|Add groupPolicyMigrationReports by posting to the groupPolicyMigrationReports collection.|
|[List groupPolicyConfigurations](../api/intune-devices-devicemanagement-list-grouppolicyconfigurations.md)|[groupPolicyConfiguration](../resources/groupPolicyConfiguration.md) collection|Get the groupPolicyConfigurations from the groupPolicyConfigurations navigation property.|
|[Add groupPolicyConfigurations](../api/intune-devices-devicemanagement-post-grouppolicyconfigurations.md)|[groupPolicyConfiguration](../resources/groupPolicyConfiguration.md)|Add groupPolicyConfigurations by posting to the groupPolicyConfigurations collection.|
|[List groupPolicyDefinitions](../api/intune-devices-devicemanagement-list-grouppolicydefinitions.md)|[groupPolicyDefinition](../resources/groupPolicyDefinition.md) collection|Get the groupPolicyDefinitions from the groupPolicyDefinitions navigation property.|
|[Add groupPolicyDefinitions](../api/intune-devices-devicemanagement-post-grouppolicydefinitions.md)|[groupPolicyDefinition](../resources/groupPolicyDefinition.md)|Add groupPolicyDefinitions by posting to the groupPolicyDefinitions collection.|
|[List groupPolicyDefinitionFiles](../api/intune-devices-devicemanagement-list-grouppolicydefinitionfiles.md)|[groupPolicyDefinitionFile](../resources/groupPolicyDefinitionFile.md) collection|Get the groupPolicyDefinitionFiles from the groupPolicyDefinitionFiles navigation property.|
|[Add groupPolicyDefinitionFiles](../api/intune-devices-devicemanagement-post-grouppolicydefinitionfiles.md)|[groupPolicyDefinitionFile](../resources/groupPolicyDefinitionFile.md)|Add groupPolicyDefinitionFiles by posting to the groupPolicyDefinitionFiles collection.|
|[List notificationMessageTemplates](../api/intune-devices-devicemanagement-list-notificationmessagetemplates.md)|[notificationMessageTemplate](../resources/notificationMessageTemplate.md) collection|Get the notificationMessageTemplates from the notificationMessageTemplates navigation property.|
|[Add notificationMessageTemplates](../api/intune-devices-devicemanagement-post-notificationmessagetemplates.md)|[notificationMessageTemplate](../resources/notificationMessageTemplate.md)|Add notificationMessageTemplates by posting to the notificationMessageTemplates collection.|
|[List domainJoinConnectors](../api/intune-devices-devicemanagement-list-domainjoinconnectors.md)|[deviceManagementDomainJoinConnector](../resources/deviceManagementDomainJoinConnector.md) collection|Get the deviceManagementDomainJoinConnectors from the domainJoinConnectors navigation property.|
|[Add domainJoinConnectors](../api/intune-devices-devicemanagement-post-domainjoinconnectors.md)|[deviceManagementDomainJoinConnector](../resources/deviceManagementDomainJoinConnector.md)|Add domainJoinConnectors by posting to the domainJoinConnectors collection.|
|[List roleDefinitions](../api/intune-devices-devicemanagement-list-roledefinitions.md)|[roleDefinition](../resources/roleDefinition.md) collection|Get the roleDefinitions from the roleDefinitions navigation property.|
|[Add roleDefinitions](../api/intune-devices-devicemanagement-post-roledefinitions.md)|[roleDefinition](../resources/roleDefinition.md)|Add roleDefinitions by posting to the roleDefinitions collection.|
|[List roleAssignments](../api/intune-devices-devicemanagement-list-roleassignments.md)|[deviceAndAppManagementRoleAssignment](../resources/deviceAndAppManagementRoleAssignment.md) collection|Get the deviceAndAppManagementRoleAssignments from the roleAssignments navigation property.|
|[Add roleAssignments](../api/intune-devices-devicemanagement-post-roleassignments.md)|[deviceAndAppManagementRoleAssignment](../resources/deviceAndAppManagementRoleAssignment.md)|Add roleAssignments by posting to the roleAssignments collection.|
|[List roleScopeTags](../api/intune-devices-devicemanagement-list-rolescopetags.md)|[roleScopeTag](../resources/roleScopeTag.md) collection|Get the roleScopeTags from the roleScopeTags navigation property.|
|[Add roleScopeTags](../api/intune-devices-devicemanagement-post-rolescopetags.md)|[roleScopeTag](../resources/roleScopeTag.md)|Add roleScopeTags by posting to the roleScopeTags collection.|
|[List resourceOperations](../api/intune-devices-devicemanagement-list-resourceoperations.md)|[resourceOperation](../resources/resourceOperation.md) collection|Get the resourceOperations from the resourceOperations navigation property.|
|[Add resourceOperations](../api/intune-devices-devicemanagement-post-resourceoperations.md)|[resourceOperation](../resources/resourceOperation.md)|Add resourceOperations by posting to the resourceOperations collection.|
|[List remoteAssistancePartners](../api/intune-devices-devicemanagement-list-remoteassistancepartners.md)|[remoteAssistancePartner](../resources/remoteAssistancePartner.md) collection|Get the remoteAssistancePartners from the remoteAssistancePartners navigation property.|
|[Add remoteAssistancePartners](../api/intune-devices-devicemanagement-post-remoteassistancepartners.md)|[remoteAssistancePartner](../resources/remoteAssistancePartner.md)|Add remoteAssistancePartners by posting to the remoteAssistancePartners collection.|
|[Get deviceManagementReports](../api/devicemanagementreports-get.md)|[deviceManagementReports](../resources/deviceManagementReports.md)|Read properties and relationships of the [deviceManagementReports](../resources/devicemanagementreports.md) object.|
|[List embeddedSIMActivationCodePools](../api/intune-devices-devicemanagement-list-embeddedsimactivationcodepools.md)|[embeddedSIMActivationCodePool](../resources/embeddedSIMActivationCodePool.md) collection|Get the embeddedSIMActivationCodePools from the embeddedSIMActivationCodePools navigation property.|
|[Add embeddedSIMActivationCodePools](../api/intune-devices-devicemanagement-post-embeddedsimactivationcodepools.md)|[embeddedSIMActivationCodePool](../resources/embeddedSIMActivationCodePool.md)|Add embeddedSIMActivationCodePools by posting to the embeddedSIMActivationCodePools collection.|
|[List telecomExpenseManagementPartners](../api/intune-devices-devicemanagement-list-telecomexpensemanagementpartners.md)|[telecomExpenseManagementPartner](../resources/telecomExpenseManagementPartner.md) collection|Get the telecomExpenseManagementPartners from the telecomExpenseManagementPartners navigation property.|
|[Add telecomExpenseManagementPartners](../api/intune-devices-devicemanagement-post-telecomexpensemanagementpartners.md)|[telecomExpenseManagementPartner](../resources/telecomExpenseManagementPartner.md)|Add telecomExpenseManagementPartners by posting to the telecomExpenseManagementPartners collection.|
|[List troubleshootingEvents](../api/intune-devices-devicemanagement-list-troubleshootingevents.md)|[deviceManagementTroubleshootingEvent](../resources/deviceManagementTroubleshootingEvent.md) collection|Get the deviceManagementTroubleshootingEvents from the troubleshootingEvents navigation property.|
|[Add troubleshootingEvents](../api/intune-devices-devicemanagement-post-troubleshootingevents.md)|[deviceManagementTroubleshootingEvent](../resources/deviceManagementTroubleshootingEvent.md)|Add troubleshootingEvents by posting to the troubleshootingEvents collection.|
|[List autopilotEvents](../api/intune-devices-devicemanagement-list-autopilotevents.md)|[deviceManagementAutopilotEvent](../resources/deviceManagementAutopilotEvent.md) collection|Get the deviceManagementAutopilotEvents from the autopilotEvents navigation property.|
|[Add autopilotEvents](../api/intune-devices-devicemanagement-post-autopilotevents.md)|[deviceManagementAutopilotEvent](../resources/deviceManagementAutopilotEvent.md)|Add autopilotEvents by posting to the autopilotEvents collection.|
|[List windowsFeatureUpdateProfiles](../api/intune-devices-devicemanagement-list-windowsfeatureupdateprofiles.md)|[windowsFeatureUpdateProfile](../resources/windowsFeatureUpdateProfile.md) collection|Get the windowsFeatureUpdateProfiles from the windowsFeatureUpdateProfiles navigation property.|
|[Add windowsFeatureUpdateProfiles](../api/intune-devices-devicemanagement-post-windowsfeatureupdateprofiles.md)|[windowsFeatureUpdateProfile](../resources/windowsFeatureUpdateProfile.md)|Add windowsFeatureUpdateProfiles by posting to the windowsFeatureUpdateProfiles collection.|
|[List windowsInformationProtectionAppLearningSummaries](../api/intune-devices-devicemanagement-list-windowsinformationprotectionapplearningsummaries.md)|[windowsInformationProtectionAppLearningSummary](../resources/windowsInformationProtectionAppLearningSummary.md) collection|Get the windowsInformationProtectionAppLearningSummaries from the windowsInformationProtectionAppLearningSummaries navigation property.|
|[Add windowsInformationProtectionAppLearningSummaries](../api/intune-devices-devicemanagement-post-windowsinformationprotectionapplearningsummaries.md)|[windowsInformationProtectionAppLearningSummary](../resources/windowsInformationProtectionAppLearningSummary.md)|Add windowsInformationProtectionAppLearningSummaries by posting to the windowsInformationProtectionAppLearningSummaries collection.|
|[List windowsInformationProtectionNetworkLearningSummaries](../api/intune-devices-devicemanagement-list-windowsinformationprotectionnetworklearningsummaries.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/windowsInformationProtectionNetworkLearningSummary.md) collection|Get the windowsInformationProtectionNetworkLearningSummaries from the windowsInformationProtectionNetworkLearningSummaries navigation property.|
|[Add windowsInformationProtectionNetworkLearningSummaries](../api/intune-devices-devicemanagement-post-windowsinformationprotectionnetworklearningsummaries.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/windowsInformationProtectionNetworkLearningSummary.md)|Add windowsInformationProtectionNetworkLearningSummaries by posting to the windowsInformationProtectionNetworkLearningSummaries collection.|
|[List intuneBrandingProfiles](../api/intune-devices-devicemanagement-list-intunebrandingprofiles.md)|[intuneBrandingProfile](../resources/intuneBrandingProfile.md) collection|Get the intuneBrandingProfiles from the intuneBrandingProfiles navigation property.|
|[Add intuneBrandingProfiles](../api/intune-devices-devicemanagement-post-intunebrandingprofiles.md)|[intuneBrandingProfile](../resources/intuneBrandingProfile.md)|Add intuneBrandingProfiles by posting to the intuneBrandingProfiles collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountMoveCompletionDateTime|DateTimeOffset|The date & time when tenant data moved between scaleunits.|
|adminConsent|[adminConsent](../resources/intune-devices-adminConsent.md)|Admin consent information.|
|deviceComplianceReportSummarizationDateTime|DateTimeOffset|The last requested time of device compliance reporting for this account. This property is read-only.|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/intune-devices-deviceProtectionOverview.md)|Device protection overview.|
|groupPolicyObjectFiles|[groupPolicyObjectFile](../resources/groupPolicyObjectFile.md) collection|A list of Group Policy Object files uploaded.|
|id|String| Inherited from [entity](../resources/entity.md)|
|intuneAccountId|Guid|Intune Account Id for given tenant|
|intuneBrand|[intuneBrand](../resources/intuneBrand.md)|intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.|
|lastReportAggregationDateTime|DateTimeOffset|The last modified time of reporting for this account. This property is read-only.|
|legacyPcManangementEnabled|Boolean|The property to enable Non-MDM managed legacy PC management for this account. This property is read-only.|
|managedDeviceCleanupSettings|[managedDeviceCleanupSettings](../resources/intune-devices-managedDeviceCleanupSettings.md)|Device cleanup rule|
|maximumDepTokens|Int32|Maximum number of dep tokens allowed per-tenant.|
|settings|[deviceManagementSettings](../resources/deviceManagementSettings.md)|Account level settings.|
|subscriptions|Enumeration|Tenant's Subscription. Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.|
|subscriptionState|Enumeration|Tenant mobile device management subscription state. Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsMalwareOverview.md)|Malware overview for windows devices.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|advancedThreatProtectionOnboardingStateSummary|[advancedThreatProtectionOnboardingStateSummary](../resources/advancedThreatProtectionOnboardingStateSummary.md)|The summary state of ATP onboarding state for this account.|
|androidDeviceOwnerEnrollmentProfiles|[androidDeviceOwnerEnrollmentProfile](../resources/androidDeviceOwnerEnrollmentProfile.md) collection|Android device owner enrollment profile entities.|
|androidForWorkAppConfigurationSchemas|[androidForWorkAppConfigurationSchema](../resources/androidForWorkAppConfigurationSchema.md) collection|Android for Work app configuration schema entities.|
|androidForWorkEnrollmentProfiles|[androidForWorkEnrollmentProfile](../resources/androidForWorkEnrollmentProfile.md) collection|Android for Work enrollment profile entities.|
|androidForWorkSettings|[androidForWorkSettings](../resources/androidForWorkSettings.md)|The singleton Android for Work settings entity.|
|androidManagedStoreAccountEnterpriseSettings|[androidManagedStoreAccountEnterpriseSettings](../resources/androidManagedStoreAccountEnterpriseSettings.md)|The singleton Android managed store account enterprise settings entity.|
|androidManagedStoreAppConfigurationSchemas|[androidManagedStoreAppConfigurationSchema](../resources/androidManagedStoreAppConfigurationSchema.md) collection|Android Enterprise app configuration schema entities.|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune-devices-applePushNotificationCertificate.md)|Apple push notification certificate.|
|appleUserInitiatedEnrollmentProfiles|[appleUserInitiatedEnrollmentProfile](../resources/appleUserInitiatedEnrollmentProfile.md) collection|Apple user initiated enrollment profiles|
|auditEvents|[auditEvent](../resources/auditEvent.md) collection|The Audit Events|
|autopilotEvents|[deviceManagementAutopilotEvent](../resources/deviceManagementAutopilotEvent.md) collection|The list of autopilot events for the tenant.|
|cartToClassAssociations|[cartToClassAssociation](../resources/cartToClassAssociation.md) collection|The Cart To Class Associations.|
|categories|[deviceManagementSettingCategory](../resources/deviceManagementSettingCategory.md) collection|The available categories|
|complianceManagementPartners|[complianceManagementPartner](../resources/complianceManagementPartner.md) collection|The list of Compliance Management Partners configured by the tenant.|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/onPremisesConditionalAccessSettings.md)|The Exchange on premises conditional access settings. On premises conditional access will require devices to be both enrolled and compliant for mail access|
|dataSharingConsents|[dataSharingConsent](../resources/intune-devices-dataSharingConsent.md) collection|Data sharing consents.|
|depOnboardingSettings|[depOnboardingSetting](../resources/depOnboardingSetting.md) collection|This collections of multiple DEP tokens per-tenant.|
|derivedCredentials|[deviceManagementDerivedCredentialSettings](../resources/deviceManagementDerivedCredentialSettings.md) collection|Collection of Derived credential settings associated with account.|
|detectedApps|[detectedApp](../resources/intune-devices-detectedApp.md) collection|The list of detected apps associated with a device.|
|deviceCategories|[deviceCategory](../resources/deviceCategory.md) collection|The list of device categories with the tenant.|
|deviceCompliancePolicies|[deviceCompliancePolicy](../resources/deviceCompliancePolicy.md) collection|The device compliance policies.|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/deviceCompliancePolicyDeviceStateSummary.md)|The device compliance state summary for this account.|
|deviceCompliancePolicySettingStateSummaries|[deviceCompliancePolicySettingStateSummary](../resources/deviceCompliancePolicySettingStateSummary.md) collection|The summary states of compliance policy settings for this account.|
|deviceConfigurationConflictSummary|[deviceConfigurationConflictSummary](../resources/deviceConfigurationConflictSummary.md) collection|Summary of policies in conflict state for this account.|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/deviceConfigurationDeviceStateSummary.md)|The device configuration device state summary for this account.|
|deviceConfigurationRestrictedAppsViolations|[restrictedAppsViolation](../resources/restrictedAppsViolation.md) collection|Restricted apps violations for this account.|
|deviceConfigurations|[deviceConfiguration](../resources/deviceConfiguration.md) collection|The device configurations.|
|deviceConfigurationsAllManagedDeviceCertificateStates|[managedAllDeviceCertificateState](../resources/managedAllDeviceCertificateState.md) collection|Summary of all certificates for all devices.|
|deviceConfigurationUserStateSummaries|[deviceConfigurationUserStateSummary](../resources/deviceConfigurationUserStateSummary.md)|The device configuration user state summary for this account.|
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/deviceEnrollmentConfiguration.md) collection|The list of device enrollment configurations|
|deviceHealthScripts|[deviceHealthScript](../resources/intune-devices-deviceHealthScript.md) collection|The list of device health scripts associated with the tenant.|
|deviceManagementPartners|[deviceManagementPartner](../resources/deviceManagementPartner.md) collection|The list of Device Management Partners configured by the tenant.|
|deviceManagementScripts|[deviceManagementScript](../resources/intune-devices-deviceManagementScript.md) collection|The list of device management scripts associated with the tenant.|
|deviceShellScripts|[deviceShellScript](../resources/intune-devices-deviceShellScript.md) collection|The list of device shell scripts associated with the tenant.|
|domainJoinConnectors|[deviceManagementDomainJoinConnector](../resources/deviceManagementDomainJoinConnector.md) collection|A list of connector objects.|
|embeddedSIMActivationCodePools|[embeddedSIMActivationCodePool](../resources/embeddedSIMActivationCodePool.md) collection|The embedded SIM activation code pools created by this account.|
|exchangeConnectors|[deviceManagementExchangeConnector](../resources/deviceManagementExchangeConnector.md) collection|The list of Exchange Connectors configured by the tenant.|
|exchangeOnPremisesPolicies|[deviceManagementExchangeOnPremisesPolicy](../resources/deviceManagementExchangeOnPremisesPolicy.md) collection|The list of Exchange On Premisis policies configured by the tenant.|
|exchangeOnPremisesPolicy|[deviceManagementExchangeOnPremisesPolicy](../resources/deviceManagementExchangeOnPremisesPolicy.md)|The policy which controls mobile device access to Exchange On Premises|
|groupPolicyConfigurations|[groupPolicyConfiguration](../resources/groupPolicyConfiguration.md) collection|The group policy configurations created by this account.|
|groupPolicyDefinitionFiles|[groupPolicyDefinitionFile](../resources/groupPolicyDefinitionFile.md) collection|The available group policy definition files for this account.|
|groupPolicyDefinitions|[groupPolicyDefinition](../resources/groupPolicyDefinition.md) collection|The available group policy definitions for this account.|
|groupPolicyMigrationReports|[groupPolicyMigrationReport](../resources/groupPolicyMigrationReport.md) collection|A list of Group Policy migration reports.|
|importedDeviceIdentities|[importedDeviceIdentity](../resources/importedDeviceIdentity.md) collection|The imported device identities.|
|importedWindowsAutopilotDeviceIdentities|[importedWindowsAutopilotDeviceIdentity](../resources/importedWindowsAutopilotDeviceIdentity.md) collection|Collection of imported Windows autopilot devices.|
|intents|[deviceManagementIntent](../resources/deviceManagementIntent.md) collection|The device management intents|
|intuneBrandingProfiles|[intuneBrandingProfile](../resources/intuneBrandingProfile.md) collection|Intune branding profiles targeted to AAD groups|
|iosUpdateStatuses|[iosUpdateDeviceStatus](../resources/iosUpdateDeviceStatus.md) collection|The IOS software update installation statuses for this account.|
|managedDeviceEncryptionStates|[managedDeviceEncryptionState](../resources/managedDeviceEncryptionState.md) collection|Encryption report for devices in this account|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-managedDeviceOverview.md)|Device overview|
|managedDevices|[managedDevice](../resources/intune-devices-managedDevice.md) collection|The list of managed devices.|
|managementConditions|[managementCondition](../resources/managementCondition.md) collection|The management conditions associated with device management of the company.|
|managementConditionStatements|[managementConditionStatement](../resources/managementConditionStatement.md) collection|The management condition statements associated with device management of the company.|
|mobileAppTroubleshootingEvents|[mobileAppTroubleshootingEvent](../resources/mobileAppTroubleshootingEvent.md) collection|The collection property of MobileAppTroubleshootingEvent.|
|mobileThreatDefenseConnectors|[mobileThreatDefenseConnector](../resources/mobileThreatDefenseConnector.md) collection|The list of Mobile threat Defense connectors configured by the tenant.|
|ndesConnectors|[ndesConnector](../resources/ndesConnector.md) collection|The collection of Ndes connectors for this account.|
|notificationMessageTemplates|[notificationMessageTemplate](../resources/notificationMessageTemplate.md) collection|The Notification Message Templates.|
|remoteActionAudits|[remoteActionAudit](../resources/intune-devices-remoteActionAudit.md) collection|The list of device remote action audits with the tenant.|
|remoteAssistancePartners|[remoteAssistancePartner](../resources/remoteAssistancePartner.md) collection|The remote assist partners.|
|reports|[deviceManagementReports](../resources/deviceManagementReports.md)|Reports singleton|
|resourceOperations|[resourceOperation](../resources/resourceOperation.md) collection|The Resource Operations.|
|roleAssignments|[deviceAndAppManagementRoleAssignment](../resources/deviceAndAppManagementRoleAssignment.md) collection|The Role Assignments.|
|roleDefinitions|[roleDefinition](../resources/roleDefinition.md) collection|The Role Definitions.|
|roleScopeTags|[roleScopeTag](../resources/roleScopeTag.md) collection|The Role Scope Tags.|
|settingDefinitions|[deviceManagementSettingDefinition](../resources/deviceManagementSettingDefinition.md) collection|The device management intent setting definitions|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/softwareUpdateStatusSummary.md)|The software update status summary.|
|telecomExpenseManagementPartners|[telecomExpenseManagementPartner](../resources/telecomExpenseManagementPartner.md) collection|The telecom expense management partners.|
|templates|[deviceManagementTemplate](../resources/deviceManagementTemplate.md) collection|The available templates|
|termsAndConditions|[termsAndConditions](../resources/termsAndConditions.md) collection|The terms and conditions associated with device management of the company.|
|troubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/deviceManagementTroubleshootingEvent.md) collection|The list of troubleshooting events for the tenant.|
|userExperienceAnalyticsBaselines|[userExperienceAnalyticsBaseline](../resources/intune-devices-userExperienceAnalyticsBaseline.md) collection|User experience analytics baselines|
|userExperienceAnalyticsCategories|[userExperienceAnalyticsCategory](../resources/intune-devices-userExperienceAnalyticsCategory.md) collection|User experience analytics categories|
|userExperienceAnalyticsDevicePerformance|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userExperienceAnalyticsDevicePerformance.md) collection|User experience analytics device performance|
|userExperienceAnalyticsDeviceStartupHistory|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userExperienceAnalyticsDeviceStartupHistory.md) collection|User experience analytics device Startup History|
|userExperienceAnalyticsOverview|[userExperienceAnalyticsOverview](../resources/intune-devices-userExperienceAnalyticsOverview.md)|User experience analytics overview|
|userExperienceAnalyticsRegressionSummary|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userExperienceAnalyticsRegressionSummary.md)|User experience analytics regression summary|
|userPfxCertificates|[userPFXCertificate](../resources/userPFXCertificate.md) collection|Collection of PFX certificates associated with a user.|
|windowsAutopilotDeploymentProfiles|[windowsAutopilotDeploymentProfile](../resources/windowsAutopilotDeploymentProfile.md) collection|Windows auto pilot deployment profiles|
|windowsAutopilotDeviceIdentities|[windowsAutopilotDeviceIdentity](../resources/windowsAutopilotDeviceIdentity.md) collection|The Windows autopilot device identities contained collection.|
|windowsAutopilotSettings|[windowsAutopilotSettings](../resources/windowsAutopilotSettings.md)|The Windows autopilot account settings.|
|windowsFeatureUpdateProfiles|[windowsFeatureUpdateProfile](../resources/windowsFeatureUpdateProfile.md) collection|A collection of windows feature update profiles|
|windowsInformationProtectionAppLearningSummaries|[windowsInformationProtectionAppLearningSummary](../resources/windowsInformationProtectionAppLearningSummary.md) collection|The windows information protection app learning summaries.|
|windowsInformationProtectionNetworkLearningSummaries|[windowsInformationProtectionNetworkLearningSummary](../resources/windowsInformationProtectionNetworkLearningSummary.md) collection|The windows information protection network learning summaries.|
|windowsMalwareInformation|[windowsMalwareInformation](../resources/intune-devices-windowsMalwareInformation.md) collection|The list of affected malware in the tenant.|

## JSON Representation
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
    "androidDeviceAdministratorEnrollmentEnabled": true
  },
  "maximumDepTokens": 1024,
  "intuneAccountId": "Guid",
  "lastReportAggregationDateTime": "String (timestamp)",
  "deviceComplianceReportSummarizationDateTime": "String (timestamp)",
  "legacyPcManangementEnabled": true,
  "intuneBrand": {
    "@odata.type": "microsoft.graph.intuneBrand",
    "darkBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent"
    },
    "showNameNextToLogo": true
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
        "@odata.type": "microsoft.graph.windowsMalwareCategoryCount",
        "category": "String"
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
  "accountMoveCompletionDateTime": "String (timestamp)",
  "groupPolicyObjectFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyObjectFile",
      "ouDistinguishedName": "String",
      "content": "String"
    }
  ]
}
```

