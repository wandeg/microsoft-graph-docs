---
title: "deviceManagement resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagement resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagement](../api/devicemanagement-get.md)|[deviceManagement](../resources/devicemanagement.md)|Read properties and relationships of the [deviceManagement](../resources/devicemanagement.md) object.|
|[Update deviceManagement](../api/devicemanagement-update.md)|[deviceManagement](../resources/devicemanagement.md)|Update the properties of a [deviceManagement](../resources/devicemanagement.md) object.|
|[enableLegacyPcManagement](../api/devicemanagement-enablelegacypcmanagement.md)|None||
|[enableAndroidDeviceAdministratorEnrollment](../api/devicemanagement-enableandroiddeviceadministratorenrollment.md)|None||
|[verifyWindowsEnrollmentAutoDiscovery](../api/devicemanagement-verifywindowsenrollmentautodiscovery.md)|Boolean||
|[sendCustomNotificationToCompanyPortal](../api/devicemanagement-sendcustomnotificationtocompanyportal.md)|None||
|[getEffectivePermissions](../api/devicemanagement-geteffectivepermissions.md)|String collection||
|[getEffectivePermissions](../api/devicemanagement-geteffectivepermissions.md)|[rolePermission](../resources/rolepermission.md) collection||
|[getRoleScopeTagsByResource](../api/devicemanagement-getrolescopetagsbyresource.md)|[roleScopeTag](../resources/rolescopetag.md) collection||
|[getRoleScopeTagsByIds](../api/devicemanagement-getrolescopetagsbyids.md)|[roleScopeTag](../resources/rolescopetag.md) collection||
|[getAssignedRoleDetails](../api/devicemanagement-getassignedroledetails.md)|[deviceAndAppManagementAssignedRoleDetails](../resources/deviceandappmanagementassignedroledetails.md)||
|[scopedForResource](../api/devicemanagement-scopedforresource.md)|Boolean||
|[List auditEvents](../api/devicemanagement-list-auditevents.md)|[auditEvent](../resources/auditevent.md) collection|Get the auditEvents from the auditEvents navigation property.|
|[Add auditEvents](../api/devicemanagement-post-auditevents.md)|[auditEvent](../resources/auditevent.md)|Add auditEvents by posting to the auditEvents collection.|
|[Get androidForWorkSettings](../api/androidforworksettings-get.md)|[androidForWorkSettings](../resources/androidforworksettings.md)|Read properties and relationships of the [androidForWorkSettings](../resources/androidforworksettings.md) object.|
|[List androidForWorkAppConfigurationSchemas](../api/devicemanagement-list-androidforworkappconfigurationschemas.md)|[androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md) collection|Get the androidForWorkAppConfigurationSchemas from the androidForWorkAppConfigurationSchemas navigation property.|
|[Add androidForWorkAppConfigurationSchemas](../api/devicemanagement-post-androidforworkappconfigurationschemas.md)|[androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md)|Add androidForWorkAppConfigurationSchemas by posting to the androidForWorkAppConfigurationSchemas collection.|
|[List androidForWorkEnrollmentProfiles](../api/devicemanagement-list-androidforworkenrollmentprofiles.md)|[androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) collection|Get the androidForWorkEnrollmentProfiles from the androidForWorkEnrollmentProfiles navigation property.|
|[Add androidForWorkEnrollmentProfiles](../api/devicemanagement-post-androidforworkenrollmentprofiles.md)|[androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md)|Add androidForWorkEnrollmentProfiles by posting to the androidForWorkEnrollmentProfiles collection.|
|[Get androidManagedStoreAccountEnterpriseSettings](../api/androidmanagedstoreaccountenterprisesettings-get.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/androidmanagedstoreaccountenterprisesettings.md)|Read properties and relationships of the [androidManagedStoreAccountEnterpriseSettings](../resources/androidmanagedstoreaccountenterprisesettings.md) object.|
|[List androidManagedStoreAppConfigurationSchemas](../api/devicemanagement-list-androidmanagedstoreappconfigurationschemas.md)|[androidManagedStoreAppConfigurationSchema](../resources/androidmanagedstoreappconfigurationschema.md) collection|Get the androidManagedStoreAppConfigurationSchemas from the androidManagedStoreAppConfigurationSchemas navigation property.|
|[Add androidManagedStoreAppConfigurationSchemas](../api/devicemanagement-post-androidmanagedstoreappconfigurationschemas.md)|[androidManagedStoreAppConfigurationSchema](../resources/androidmanagedstoreappconfigurationschema.md)|Add androidManagedStoreAppConfigurationSchemas by posting to the androidManagedStoreAppConfigurationSchemas collection.|
|[List androidDeviceOwnerEnrollmentProfiles](../api/devicemanagement-list-androiddeviceownerenrollmentprofiles.md)|[androidDeviceOwnerEnrollmentProfile](../resources/androiddeviceownerenrollmentprofile.md) collection|Get the androidDeviceOwnerEnrollmentProfiles from the androidDeviceOwnerEnrollmentProfiles navigation property.|
|[Add androidDeviceOwnerEnrollmentProfiles](../api/devicemanagement-post-androiddeviceownerenrollmentprofiles.md)|[androidDeviceOwnerEnrollmentProfile](../resources/androiddeviceownerenrollmentprofile.md)|Add androidDeviceOwnerEnrollmentProfiles by posting to the androidDeviceOwnerEnrollmentProfiles collection.|
|[List termsAndConditions](../api/devicemanagement-list-termsandconditions.md)|[termsAndConditions](../resources/termsandconditions.md) collection|Get the termsAndConditionses from the termsAndConditions navigation property.|
|[Add termsAndConditions](../api/devicemanagement-post-termsandconditions.md)|[termsAndConditions](../resources/termsandconditions.md)|Add termsAndConditions by posting to the termsAndConditions collection.|
|[List deviceConfigurations](../api/devicemanagement-list-deviceconfigurations.md)|[deviceConfiguration](../resources/deviceconfiguration.md) collection|Get the deviceConfigurations from the deviceConfigurations navigation property.|
|[Add deviceConfigurations](../api/devicemanagement-post-deviceconfigurations.md)|[deviceConfiguration](../resources/deviceconfiguration.md)|Add deviceConfigurations by posting to the deviceConfigurations collection.|
|[List deviceCompliancePolicies](../api/devicemanagement-list-devicecompliancepolicies.md)|[deviceCompliancePolicy](../resources/devicecompliancepolicy.md) collection|Get the deviceCompliancePolicies from the deviceCompliancePolicies navigation property.|
|[Add deviceCompliancePolicies](../api/devicemanagement-post-devicecompliancepolicies.md)|[deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|Add deviceCompliancePolicies by posting to the deviceCompliancePolicies collection.|
|[Get softwareUpdateStatusSummary](../api/softwareupdatestatussummary-get.md)|[softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md)|Read properties and relationships of the [softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md) object.|
|[Get deviceCompliancePolicyDeviceStateSummary](../api/devicecompliancepolicydevicestatesummary-get.md)|[deviceCompliancePolicyDeviceStateSummary](../resources/devicecompliancepolicydevicestatesummary.md)|Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/devicecompliancepolicydevicestatesummary.md) object.|
|[List deviceCompliancePolicySettingStateSummaries](../api/devicemanagement-list-devicecompliancepolicysettingstatesummaries.md)|[deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md) collection|Get the deviceCompliancePolicySettingStateSummaries from the deviceCompliancePolicySettingStateSummaries navigation property.|
|[Add deviceCompliancePolicySettingStateSummaries](../api/devicemanagement-post-devicecompliancepolicysettingstatesummaries.md)|[deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md)|Add deviceCompliancePolicySettingStateSummaries by posting to the deviceCompliancePolicySettingStateSummaries collection.|
|[Get advancedThreatProtectionOnboardingStateSummary](../api/advancedthreatprotectiononboardingstatesummary-get.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md)|Read properties and relationships of the [advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md) object.|
|[Get deviceConfigurationDeviceStateSummary](../api/deviceconfigurationdevicestatesummary-get.md)|[deviceConfigurationDeviceStateSummary](../resources/deviceconfigurationdevicestatesummary.md)|Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/deviceconfigurationdevicestatesummary.md) object.|
|[Get deviceConfigurationUserStateSummary](../api/deviceconfigurationuserstatesummary-get.md)|[deviceConfigurationUserStateSummary](../resources/deviceconfigurationuserstatesummary.md)|Read properties and relationships of the [deviceConfigurationUserStateSummary](../resources/deviceconfigurationuserstatesummary.md) object.|
|[List cartToClassAssociations](../api/devicemanagement-list-carttoclassassociations.md)|[cartToClassAssociation](../resources/carttoclassassociation.md) collection|Get the cartToClassAssociations from the cartToClassAssociations navigation property.|
|[Add cartToClassAssociations](../api/devicemanagement-post-carttoclassassociations.md)|[cartToClassAssociation](../resources/carttoclassassociation.md)|Add cartToClassAssociations by posting to the cartToClassAssociations collection.|
|[List iosUpdateStatuses](../api/devicemanagement-list-iosupdatestatuses.md)|[iosUpdateDeviceStatus](../resources/iosupdatedevicestatus.md) collection|Get the iosUpdateDeviceStatuses from the iosUpdateStatuses navigation property.|
|[Add iosUpdateStatuses](../api/devicemanagement-post-iosupdatestatuses.md)|[iosUpdateDeviceStatus](../resources/iosupdatedevicestatus.md)|Add iosUpdateStatuses by posting to the iosUpdateStatuses collection.|
|[List ndesConnectors](../api/devicemanagement-list-ndesconnectors.md)|[ndesConnector](../resources/ndesconnector.md) collection|Get the ndesConnectors from the ndesConnectors navigation property.|
|[Add ndesConnectors](../api/devicemanagement-post-ndesconnectors.md)|[ndesConnector](../resources/ndesconnector.md)|Add ndesConnectors by posting to the ndesConnectors collection.|
|[List deviceConfigurationRestrictedAppsViolations](../api/devicemanagement-list-deviceconfigurationrestrictedappsviolations.md)|[restrictedAppsViolation](../resources/restrictedappsviolation.md) collection|Get the restrictedAppsViolations from the deviceConfigurationRestrictedAppsViolations navigation property.|
|[Add deviceConfigurationRestrictedAppsViolations](../api/devicemanagement-post-deviceconfigurationrestrictedappsviolations.md)|[restrictedAppsViolation](../resources/restrictedappsviolation.md)|Add deviceConfigurationRestrictedAppsViolations by posting to the deviceConfigurationRestrictedAppsViolations collection.|
|[List managedDeviceEncryptionStates](../api/devicemanagement-list-manageddeviceencryptionstates.md)|[managedDeviceEncryptionState](../resources/manageddeviceencryptionstate.md) collection|Get the managedDeviceEncryptionStates from the managedDeviceEncryptionStates navigation property.|
|[Add managedDeviceEncryptionStates](../api/devicemanagement-post-manageddeviceencryptionstates.md)|[managedDeviceEncryptionState](../resources/manageddeviceencryptionstate.md)|Add managedDeviceEncryptionStates by posting to the managedDeviceEncryptionStates collection.|
|[List deviceConfigurationConflictSummary](../api/devicemanagement-list-deviceconfigurationconflictsummary.md)|[deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md) collection|Get the deviceConfigurationConflictSummaries from the deviceConfigurationConflictSummary navigation property.|
|[Add deviceConfigurationConflictSummary](../api/devicemanagement-post-deviceconfigurationconflictsummary.md)|[deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md)|Add deviceConfigurationConflictSummary by posting to the deviceConfigurationConflictSummary collection.|
|[List deviceConfigurationsAllManagedDeviceCertificateStates](../api/devicemanagement-list-deviceconfigurationsallmanageddevicecertificatestates.md)|[managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md) collection|Get the managedAllDeviceCertificateStates from the deviceConfigurationsAllManagedDeviceCertificateStates navigation property.|
|[Add deviceConfigurationsAllManagedDeviceCertificateStates](../api/devicemanagement-post-deviceconfigurationsallmanageddevicecertificatestates.md)|[managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md)|Add deviceConfigurationsAllManagedDeviceCertificateStates by posting to the deviceConfigurationsAllManagedDeviceCertificateStates collection.|
|[List deviceCategories](../api/devicemanagement-list-devicecategories.md)|[deviceCategory](../resources/devicecategory.md) collection|Get the deviceCategories from the deviceCategories navigation property.|
|[Add deviceCategories](../api/devicemanagement-post-devicecategories.md)|[deviceCategory](../resources/devicecategory.md)|Add deviceCategories by posting to the deviceCategories collection.|
|[List exchangeConnectors](../api/devicemanagement-list-exchangeconnectors.md)|[deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) collection|Get the deviceManagementExchangeConnectors from the exchangeConnectors navigation property.|
|[Add exchangeConnectors](../api/devicemanagement-post-exchangeconnectors.md)|[deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md)|Add exchangeConnectors by posting to the exchangeConnectors collection.|
|[List deviceEnrollmentConfigurations](../api/devicemanagement-list-deviceenrollmentconfigurations.md)|[deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md) collection|Get the deviceEnrollmentConfigurations from the deviceEnrollmentConfigurations navigation property.|
|[Add deviceEnrollmentConfigurations](../api/devicemanagement-post-deviceenrollmentconfigurations.md)|[deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|Add deviceEnrollmentConfigurations by posting to the deviceEnrollmentConfigurations collection.|
|[Get deviceManagementExchangeOnPremisesPolicy](../api/devicemanagementexchangeonpremisespolicy-get.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md)|Read properties and relationships of the [deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md) object.|
|[List exchangeOnPremisesPolicies](../api/devicemanagement-list-exchangeonpremisespolicies.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md) collection|Get the deviceManagementExchangeOnPremisesPolicies from the exchangeOnPremisesPolicies navigation property.|
|[Add exchangeOnPremisesPolicies](../api/devicemanagement-post-exchangeonpremisespolicies.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md)|Add exchangeOnPremisesPolicies by posting to the exchangeOnPremisesPolicies collection.|
|[Get onPremisesConditionalAccessSettings](../api/onpremisesconditionalaccesssettings-get.md)|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md)|Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.|
|[List mobileThreatDefenseConnectors](../api/devicemanagement-list-mobilethreatdefenseconnectors.md)|[mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) collection|Get the mobileThreatDefenseConnectors from the mobileThreatDefenseConnectors navigation property.|
|[Add mobileThreatDefenseConnectors](../api/devicemanagement-post-mobilethreatdefenseconnectors.md)|[mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md)|Add mobileThreatDefenseConnectors by posting to the mobileThreatDefenseConnectors collection.|
|[List deviceManagementPartners](../api/devicemanagement-list-devicemanagementpartners.md)|[deviceManagementPartner](../resources/devicemanagementpartner.md) collection|Get the deviceManagementPartners from the deviceManagementPartners navigation property.|
|[Add deviceManagementPartners](../api/devicemanagement-post-devicemanagementpartners.md)|[deviceManagementPartner](../resources/devicemanagementpartner.md)|Add deviceManagementPartners by posting to the deviceManagementPartners collection.|
|[List complianceManagementPartners](../api/devicemanagement-list-compliancemanagementpartners.md)|[complianceManagementPartner](../resources/compliancemanagementpartner.md) collection|Get the complianceManagementPartners from the complianceManagementPartners navigation property.|
|[Add complianceManagementPartners](../api/devicemanagement-post-compliancemanagementpartners.md)|[complianceManagementPartner](../resources/compliancemanagementpartner.md)|Add complianceManagementPartners by posting to the complianceManagementPartners collection.|
|[List intents](../api/devicemanagement-list-intents.md)|[deviceManagementIntent](../resources/devicemanagementintent.md) collection|Get the deviceManagementIntents from the intents navigation property.|
|[Add intents](../api/devicemanagement-post-intents.md)|[deviceManagementIntent](../resources/devicemanagementintent.md)|Add intents by posting to the intents collection.|
|[List settingDefinitions](../api/devicemanagement-list-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) collection|Get the deviceManagementSettingDefinitions from the settingDefinitions navigation property.|
|[Add settingDefinitions](../api/devicemanagement-post-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|Add settingDefinitions by posting to the settingDefinitions collection.|
|[List templates](../api/devicemanagement-list-templates.md)|[deviceManagementTemplate](../resources/devicemanagementtemplate.md) collection|Get the deviceManagementTemplates from the templates navigation property.|
|[Add templates](../api/devicemanagement-post-templates.md)|[deviceManagementTemplate](../resources/devicemanagementtemplate.md)|Add templates by posting to the templates collection.|
|[List categories](../api/devicemanagement-list-categories.md)|[deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) collection|Get the deviceManagementSettingCategories from the categories navigation property.|
|[Add categories](../api/devicemanagement-post-categories.md)|[deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|Add categories by posting to the categories collection.|
|[List remoteActionAudits](../api/devicemanagement-list-remoteactionaudits.md)|[remoteActionAudit](../resources/remoteactionaudit.md) collection|Get the remoteActionAudits from the remoteActionAudits navigation property.|
|[Add remoteActionAudits](../api/devicemanagement-post-remoteactionaudits.md)|[remoteActionAudit](../resources/remoteactionaudit.md)|Add remoteActionAudits by posting to the remoteActionAudits collection.|
|[Get applePushNotificationCertificate](../api/applepushnotificationcertificate-get.md)|[applePushNotificationCertificate](../resources/applepushnotificationcertificate.md)|Read properties and relationships of the [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object.|
|[List deviceManagementScripts](../api/devicemanagement-list-devicemanagementscripts.md)|[deviceManagementScript](../resources/devicemanagementscript.md) collection|Get the deviceManagementScripts from the deviceManagementScripts navigation property.|
|[Add deviceManagementScripts](../api/devicemanagement-post-devicemanagementscripts.md)|[deviceManagementScript](../resources/devicemanagementscript.md)|Add deviceManagementScripts by posting to the deviceManagementScripts collection.|
|[List deviceShellScripts](../api/devicemanagement-list-deviceshellscripts.md)|[deviceShellScript](../resources/deviceshellscript.md) collection|Get the deviceShellScripts from the deviceShellScripts navigation property.|
|[Add deviceShellScripts](../api/devicemanagement-post-deviceshellscripts.md)|[deviceShellScript](../resources/deviceshellscript.md)|Add deviceShellScripts by posting to the deviceShellScripts collection.|
|[List deviceHealthScripts](../api/devicemanagement-list-devicehealthscripts.md)|[deviceHealthScript](../resources/devicehealthscript.md) collection|Get the deviceHealthScripts from the deviceHealthScripts navigation property.|
|[Add deviceHealthScripts](../api/devicemanagement-post-devicehealthscripts.md)|[deviceHealthScript](../resources/devicehealthscript.md)|Add deviceHealthScripts by posting to the deviceHealthScripts collection.|
|[Get managedDeviceOverview](../api/manageddeviceoverview-get.md)|[managedDeviceOverview](../resources/manageddeviceoverview.md)|Read properties and relationships of the [managedDeviceOverview](../resources/manageddeviceoverview.md) object.|
|[List detectedApps](../api/devicemanagement-list-detectedapps.md)|[detectedApp](../resources/detectedapp.md) collection|Get the detectedApps from the detectedApps navigation property.|
|[Add detectedApps](../api/devicemanagement-post-detectedapps.md)|[detectedApp](../resources/detectedapp.md)|Add detectedApps by posting to the detectedApps collection.|
|[List managedDevices](../api/devicemanagement-list-manageddevices.md)|[managedDevice](../resources/manageddevice.md) collection|Get the managedDevices from the managedDevices navigation property.|
|[Add managedDevices](../api/devicemanagement-post-manageddevices.md)|[managedDevice](../resources/manageddevice.md)|Add managedDevices by posting to the managedDevices collection.|
|[List windowsMalwareInformation](../api/devicemanagement-list-windowsmalwareinformation.md)|[windowsMalwareInformation](../resources/windowsmalwareinformation.md) collection|Get the windowsMalwareInformations from the windowsMalwareInformation navigation property.|
|[Add windowsMalwareInformation](../api/devicemanagement-post-windowsmalwareinformation.md)|[windowsMalwareInformation](../resources/windowsmalwareinformation.md)|Add windowsMalwareInformation by posting to the windowsMalwareInformation collection.|
|[List dataSharingConsents](../api/devicemanagement-list-datasharingconsents.md)|[dataSharingConsent](../resources/datasharingconsent.md) collection|Get the dataSharingConsents from the dataSharingConsents navigation property.|
|[Add dataSharingConsents](../api/devicemanagement-post-datasharingconsents.md)|[dataSharingConsent](../resources/datasharingconsent.md)|Add dataSharingConsents by posting to the dataSharingConsents collection.|
|[List mobileAppTroubleshootingEvents](../api/devicemanagement-list-mobileapptroubleshootingevents.md)|[mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md) collection|Get the mobileAppTroubleshootingEvents from the mobileAppTroubleshootingEvents navigation property.|
|[Add mobileAppTroubleshootingEvents](../api/devicemanagement-post-mobileapptroubleshootingevents.md)|[mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md)|Add mobileAppTroubleshootingEvents by posting to the mobileAppTroubleshootingEvents collection.|
|[Get userExperienceAnalyticsOverview](../api/userexperienceanalyticsoverview-get.md)|[userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md)|Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md) object.|
|[List userExperienceAnalyticsBaselines](../api/devicemanagement-list-userexperienceanalyticsbaselines.md)|[userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md) collection|Get the userExperienceAnalyticsBaselines from the userExperienceAnalyticsBaselines navigation property.|
|[Add userExperienceAnalyticsBaselines](../api/devicemanagement-post-userexperienceanalyticsbaselines.md)|[userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md)|Add userExperienceAnalyticsBaselines by posting to the userExperienceAnalyticsBaselines collection.|
|[List userExperienceAnalyticsCategories](../api/devicemanagement-list-userexperienceanalyticscategories.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) collection|Get the userExperienceAnalyticsCategories from the userExperienceAnalyticsCategories navigation property.|
|[Add userExperienceAnalyticsCategories](../api/devicemanagement-post-userexperienceanalyticscategories.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|Add userExperienceAnalyticsCategories by posting to the userExperienceAnalyticsCategories collection.|
|[List userExperienceAnalyticsDevicePerformance](../api/devicemanagement-list-userexperienceanalyticsdeviceperformance.md)|[userExperienceAnalyticsDevicePerformance](../resources/userexperienceanalyticsdeviceperformance.md) collection|Get the userExperienceAnalyticsDevicePerformances from the userExperienceAnalyticsDevicePerformance navigation property.|
|[Add userExperienceAnalyticsDevicePerformance](../api/devicemanagement-post-userexperienceanalyticsdeviceperformance.md)|[userExperienceAnalyticsDevicePerformance](../resources/userexperienceanalyticsdeviceperformance.md)|Add userExperienceAnalyticsDevicePerformance by posting to the userExperienceAnalyticsDevicePerformance collection.|
|[Get userExperienceAnalyticsRegressionSummary](../api/userexperienceanalyticsregressionsummary-get.md)|[userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md)|Read properties and relationships of the [userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md) object.|
|[List userExperienceAnalyticsDeviceStartupHistory](../api/devicemanagement-list-userexperienceanalyticsdevicestartuphistory.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/userexperienceanalyticsdevicestartuphistory.md) collection|Get the userExperienceAnalyticsDeviceStartupHistories from the userExperienceAnalyticsDeviceStartupHistory navigation property.|
|[Add userExperienceAnalyticsDeviceStartupHistory](../api/devicemanagement-post-userexperienceanalyticsdevicestartuphistory.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/userexperienceanalyticsdevicestartuphistory.md)|Add userExperienceAnalyticsDeviceStartupHistory by posting to the userExperienceAnalyticsDeviceStartupHistory collection.|
|[List userExperienceAnalyticsDeviceStartupProcesses](../api/devicemanagement-list-userexperienceanalyticsdevicestartupprocesses.md)|[userExperienceAnalyticsDeviceStartupProcess](../resources/userexperienceanalyticsdevicestartupprocess.md) collection|Get the userExperienceAnalyticsDeviceStartupProcesses from the userExperienceAnalyticsDeviceStartupProcesses navigation property.|
|[Add userExperienceAnalyticsDeviceStartupProcesses](../api/devicemanagement-post-userexperienceanalyticsdevicestartupprocesses.md)|[userExperienceAnalyticsDeviceStartupProcess](../resources/userexperienceanalyticsdevicestartupprocess.md)|Add userExperienceAnalyticsDeviceStartupProcesses by posting to the userExperienceAnalyticsDeviceStartupProcesses collection.|
|[List userExperienceAnalyticsDeviceStartupProcessPerformance](../api/devicemanagement-list-userexperienceanalyticsdevicestartupprocessperformance.md)|[userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/userexperienceanalyticsdevicestartupprocessperformance.md) collection|Get the userExperienceAnalyticsDeviceStartupProcessPerformances from the userExperienceAnalyticsDeviceStartupProcessPerformance navigation property.|
|[Add userExperienceAnalyticsDeviceStartupProcessPerformance](../api/devicemanagement-post-userexperienceanalyticsdevicestartupprocessperformance.md)|[userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/userexperienceanalyticsdevicestartupprocessperformance.md)|Add userExperienceAnalyticsDeviceStartupProcessPerformance by posting to the userExperienceAnalyticsDeviceStartupProcessPerformance collection.|
|[List userExperienceAnalyticsStartupScoreHistory](../api/devicemanagement-list-userexperienceanalyticsstartupscorehistory.md)|[userExperienceAnalyticsStartupScoreHistory](../resources/userexperienceanalyticsstartupscorehistory.md) collection|Get the userExperienceAnalyticsStartupScoreHistories from the userExperienceAnalyticsStartupScoreHistory navigation property.|
|[Add userExperienceAnalyticsStartupScoreHistory](../api/devicemanagement-post-userexperienceanalyticsstartupscorehistory.md)|[userExperienceAnalyticsStartupScoreHistory](../resources/userexperienceanalyticsstartupscorehistory.md)|Add userExperienceAnalyticsStartupScoreHistory by posting to the userExperienceAnalyticsStartupScoreHistory collection.|
|[List derivedCredentials](../api/devicemanagement-list-derivedcredentials.md)|[deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) collection|Get the deviceManagementDerivedCredentialSettingses from the derivedCredentials navigation property.|
|[Add derivedCredentials](../api/devicemanagement-post-derivedcredentials.md)|[deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md)|Add derivedCredentials by posting to the derivedCredentials collection.|
|[Get windowsAutopilotSettings](../api/windowsautopilotsettings-get.md)|[windowsAutopilotSettings](../resources/windowsautopilotsettings.md)|Read properties and relationships of the [windowsAutopilotSettings](../resources/windowsautopilotsettings.md) object.|
|[List windowsAutopilotDeviceIdentities](../api/devicemanagement-list-windowsautopilotdeviceidentities.md)|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) collection|Get the windowsAutopilotDeviceIdentities from the windowsAutopilotDeviceIdentities navigation property.|
|[Add windowsAutopilotDeviceIdentities](../api/devicemanagement-post-windowsautopilotdeviceidentities.md)|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md)|Add windowsAutopilotDeviceIdentities by posting to the windowsAutopilotDeviceIdentities collection.|
|[List windowsAutopilotDeploymentProfiles](../api/devicemanagement-list-windowsautopilotdeploymentprofiles.md)|[windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md) collection|Get the windowsAutopilotDeploymentProfiles from the windowsAutopilotDeploymentProfiles navigation property.|
|[Add windowsAutopilotDeploymentProfiles](../api/devicemanagement-post-windowsautopilotdeploymentprofiles.md)|[windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md)|Add windowsAutopilotDeploymentProfiles by posting to the windowsAutopilotDeploymentProfiles collection.|
|[List importedDeviceIdentities](../api/devicemanagement-list-importeddeviceidentities.md)|[importedDeviceIdentity](../resources/importeddeviceidentity.md) collection|Get the importedDeviceIdentities from the importedDeviceIdentities navigation property.|
|[Add importedDeviceIdentities](../api/devicemanagement-post-importeddeviceidentities.md)|[importedDeviceIdentity](../resources/importeddeviceidentity.md)|Add importedDeviceIdentities by posting to the importedDeviceIdentities collection.|
|[List depOnboardingSettings](../api/devicemanagement-list-deponboardingsettings.md)|[depOnboardingSetting](../resources/deponboardingsetting.md) collection|Get the depOnboardingSettings from the depOnboardingSettings navigation property.|
|[Add depOnboardingSettings](../api/devicemanagement-post-deponboardingsettings.md)|[depOnboardingSetting](../resources/deponboardingsetting.md)|Add depOnboardingSettings by posting to the depOnboardingSettings collection.|
|[List importedWindowsAutopilotDeviceIdentities](../api/devicemanagement-list-importedwindowsautopilotdeviceidentities.md)|[importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md) collection|Get the importedWindowsAutopilotDeviceIdentities from the importedWindowsAutopilotDeviceIdentities navigation property.|
|[Add importedWindowsAutopilotDeviceIdentities](../api/devicemanagement-post-importedwindowsautopilotdeviceidentities.md)|[importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md)|Add importedWindowsAutopilotDeviceIdentities by posting to the importedWindowsAutopilotDeviceIdentities collection.|
|[List appleUserInitiatedEnrollmentProfiles](../api/devicemanagement-list-appleuserinitiatedenrollmentprofiles.md)|[appleUserInitiatedEnrollmentProfile](../resources/appleuserinitiatedenrollmentprofile.md) collection|Get the appleUserInitiatedEnrollmentProfiles from the appleUserInitiatedEnrollmentProfiles navigation property.|
|[Add appleUserInitiatedEnrollmentProfiles](../api/devicemanagement-post-appleuserinitiatedenrollmentprofiles.md)|[appleUserInitiatedEnrollmentProfile](../resources/appleuserinitiatedenrollmentprofile.md)|Add appleUserInitiatedEnrollmentProfiles by posting to the appleUserInitiatedEnrollmentProfiles collection.|
|[List managementConditions](../api/devicemanagement-list-managementconditions.md)|[managementCondition](../resources/managementcondition.md) collection|Get the managementConditions from the managementConditions navigation property.|
|[Add managementConditions](../api/devicemanagement-post-managementconditions.md)|[managementCondition](../resources/managementcondition.md)|Add managementConditions by posting to the managementConditions collection.|
|[List managementConditionStatements](../api/devicemanagement-list-managementconditionstatements.md)|[managementConditionStatement](../resources/managementconditionstatement.md) collection|Get the managementConditionStatements from the managementConditionStatements navigation property.|
|[Add managementConditionStatements](../api/devicemanagement-post-managementconditionstatements.md)|[managementConditionStatement](../resources/managementconditionstatement.md)|Add managementConditionStatements by posting to the managementConditionStatements collection.|
|[List groupPolicyObjectFiles](../api/devicemanagement-list-grouppolicyobjectfiles.md)|[groupPolicyObjectFile](../resources/grouppolicyobjectfile.md) collection|Get the groupPolicyObjectFiles from the groupPolicyObjectFiles navigation property.|
|[Add groupPolicyObjectFiles](../api/devicemanagement-post-grouppolicyobjectfiles.md)|[groupPolicyObjectFile](../resources/grouppolicyobjectfile.md)|Add groupPolicyObjectFiles by posting to the groupPolicyObjectFiles collection.|
|[List groupPolicyMigrationReports](../api/devicemanagement-list-grouppolicymigrationreports.md)|[groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) collection|Get the groupPolicyMigrationReports from the groupPolicyMigrationReports navigation property.|
|[Add groupPolicyMigrationReports](../api/devicemanagement-post-grouppolicymigrationreports.md)|[groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md)|Add groupPolicyMigrationReports by posting to the groupPolicyMigrationReports collection.|
|[List groupPolicyConfigurations](../api/devicemanagement-list-grouppolicyconfigurations.md)|[groupPolicyConfiguration](../resources/grouppolicyconfiguration.md) collection|Get the groupPolicyConfigurations from the groupPolicyConfigurations navigation property.|
|[Add groupPolicyConfigurations](../api/devicemanagement-post-grouppolicyconfigurations.md)|[groupPolicyConfiguration](../resources/grouppolicyconfiguration.md)|Add groupPolicyConfigurations by posting to the groupPolicyConfigurations collection.|
|[List groupPolicyCategories](../api/devicemanagement-list-grouppolicycategories.md)|[groupPolicyCategory](../resources/grouppolicycategory.md) collection|Get the groupPolicyCategories from the groupPolicyCategories navigation property.|
|[Add groupPolicyCategories](../api/devicemanagement-post-grouppolicycategories.md)|[groupPolicyCategory](../resources/grouppolicycategory.md)|Add groupPolicyCategories by posting to the groupPolicyCategories collection.|
|[List groupPolicyDefinitions](../api/devicemanagement-list-grouppolicydefinitions.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md) collection|Get the groupPolicyDefinitions from the groupPolicyDefinitions navigation property.|
|[Add groupPolicyDefinitions](../api/devicemanagement-post-grouppolicydefinitions.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Add groupPolicyDefinitions by posting to the groupPolicyDefinitions collection.|
|[List groupPolicyDefinitionFiles](../api/devicemanagement-list-grouppolicydefinitionfiles.md)|[groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) collection|Get the groupPolicyDefinitionFiles from the groupPolicyDefinitionFiles navigation property.|
|[Add groupPolicyDefinitionFiles](../api/devicemanagement-post-grouppolicydefinitionfiles.md)|[groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|Add groupPolicyDefinitionFiles by posting to the groupPolicyDefinitionFiles collection.|
|[List notificationMessageTemplates](../api/devicemanagement-list-notificationmessagetemplates.md)|[notificationMessageTemplate](../resources/notificationmessagetemplate.md) collection|Get the notificationMessageTemplates from the notificationMessageTemplates navigation property.|
|[Add notificationMessageTemplates](../api/devicemanagement-post-notificationmessagetemplates.md)|[notificationMessageTemplate](../resources/notificationmessagetemplate.md)|Add notificationMessageTemplates by posting to the notificationMessageTemplates collection.|
|[List domainJoinConnectors](../api/devicemanagement-list-domainjoinconnectors.md)|[deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md) collection|Get the deviceManagementDomainJoinConnectors from the domainJoinConnectors navigation property.|
|[Add domainJoinConnectors](../api/devicemanagement-post-domainjoinconnectors.md)|[deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md)|Add domainJoinConnectors by posting to the domainJoinConnectors collection.|
|[List roleDefinitions](../api/devicemanagement-list-roledefinitions.md)|[roleDefinition](../resources/roledefinition.md) collection|Get the roleDefinitions from the roleDefinitions navigation property.|
|[Add roleDefinitions](../api/devicemanagement-post-roledefinitions.md)|[roleDefinition](../resources/roledefinition.md)|Add roleDefinitions by posting to the roleDefinitions collection.|
|[List roleAssignments](../api/devicemanagement-list-roleassignments.md)|[deviceAndAppManagementRoleAssignment](../resources/deviceandappmanagementroleassignment.md) collection|Get the deviceAndAppManagementRoleAssignments from the roleAssignments navigation property.|
|[Add roleAssignments](../api/devicemanagement-post-roleassignments.md)|[deviceAndAppManagementRoleAssignment](../resources/deviceandappmanagementroleassignment.md)|Add roleAssignments by posting to the roleAssignments collection.|
|[List roleScopeTags](../api/devicemanagement-list-rolescopetags.md)|[roleScopeTag](../resources/rolescopetag.md) collection|Get the roleScopeTags from the roleScopeTags navigation property.|
|[Add roleScopeTags](../api/devicemanagement-post-rolescopetags.md)|[roleScopeTag](../resources/rolescopetag.md)|Add roleScopeTags by posting to the roleScopeTags collection.|
|[List resourceOperations](../api/devicemanagement-list-resourceoperations.md)|[resourceOperation](../resources/resourceoperation.md) collection|Get the resourceOperations from the resourceOperations navigation property.|
|[Add resourceOperations](../api/devicemanagement-post-resourceoperations.md)|[resourceOperation](../resources/resourceoperation.md)|Add resourceOperations by posting to the resourceOperations collection.|
|[List remoteAssistancePartners](../api/devicemanagement-list-remoteassistancepartners.md)|[remoteAssistancePartner](../resources/remoteassistancepartner.md) collection|Get the remoteAssistancePartners from the remoteAssistancePartners navigation property.|
|[Add remoteAssistancePartners](../api/devicemanagement-post-remoteassistancepartners.md)|[remoteAssistancePartner](../resources/remoteassistancepartner.md)|Add remoteAssistancePartners by posting to the remoteAssistancePartners collection.|
|[Get deviceManagementReports](../api/devicemanagementreports-get.md)|[deviceManagementReports](../resources/devicemanagementreports.md)|Read properties and relationships of the [deviceManagementReports](../resources/devicemanagementreports.md) object.|
|[List telecomExpenseManagementPartners](../api/devicemanagement-list-telecomexpensemanagementpartners.md)|[telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) collection|Get the telecomExpenseManagementPartners from the telecomExpenseManagementPartners navigation property.|
|[Add telecomExpenseManagementPartners](../api/devicemanagement-post-telecomexpensemanagementpartners.md)|[telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md)|Add telecomExpenseManagementPartners by posting to the telecomExpenseManagementPartners collection.|
|[List embeddedSIMActivationCodePools](../api/devicemanagement-list-embeddedsimactivationcodepools.md)|[embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md) collection|Get the embeddedSIMActivationCodePools from the embeddedSIMActivationCodePools navigation property.|
|[Add embeddedSIMActivationCodePools](../api/devicemanagement-post-embeddedsimactivationcodepools.md)|[embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md)|Add embeddedSIMActivationCodePools by posting to the embeddedSIMActivationCodePools collection.|
|[List troubleshootingEvents](../api/devicemanagement-list-troubleshootingevents.md)|[deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md) collection|Get the deviceManagementTroubleshootingEvents from the troubleshootingEvents navigation property.|
|[Add troubleshootingEvents](../api/devicemanagement-post-troubleshootingevents.md)|[deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|Add troubleshootingEvents by posting to the troubleshootingEvents collection.|
|[List autopilotEvents](../api/devicemanagement-list-autopilotevents.md)|[deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) collection|Get the deviceManagementAutopilotEvents from the autopilotEvents navigation property.|
|[Add autopilotEvents](../api/devicemanagement-post-autopilotevents.md)|[deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md)|Add autopilotEvents by posting to the autopilotEvents collection.|
|[List windowsFeatureUpdateProfiles](../api/devicemanagement-list-windowsfeatureupdateprofiles.md)|[windowsFeatureUpdateProfile](../resources/windowsfeatureupdateprofile.md) collection|Get the windowsFeatureUpdateProfiles from the windowsFeatureUpdateProfiles navigation property.|
|[Add windowsFeatureUpdateProfiles](../api/devicemanagement-post-windowsfeatureupdateprofiles.md)|[windowsFeatureUpdateProfile](../resources/windowsfeatureupdateprofile.md)|Add windowsFeatureUpdateProfiles by posting to the windowsFeatureUpdateProfiles collection.|
|[List windowsInformationProtectionAppLearningSummaries](../api/devicemanagement-list-windowsinformationprotectionapplearningsummaries.md)|[windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md) collection|Get the windowsInformationProtectionAppLearningSummaries from the windowsInformationProtectionAppLearningSummaries navigation property.|
|[Add windowsInformationProtectionAppLearningSummaries](../api/devicemanagement-post-windowsinformationprotectionapplearningsummaries.md)|[windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md)|Add windowsInformationProtectionAppLearningSummaries by posting to the windowsInformationProtectionAppLearningSummaries collection.|
|[List windowsInformationProtectionNetworkLearningSummaries](../api/devicemanagement-list-windowsinformationprotectionnetworklearningsummaries.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md) collection|Get the windowsInformationProtectionNetworkLearningSummaries from the windowsInformationProtectionNetworkLearningSummaries navigation property.|
|[Add windowsInformationProtectionNetworkLearningSummaries](../api/devicemanagement-post-windowsinformationprotectionnetworklearningsummaries.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md)|Add windowsInformationProtectionNetworkLearningSummaries by posting to the windowsInformationProtectionNetworkLearningSummaries collection.|
|[List intuneBrandingProfiles](../api/devicemanagement-list-intunebrandingprofiles.md)|[intuneBrandingProfile](../resources/intunebrandingprofile.md) collection|Get the intuneBrandingProfiles from the intuneBrandingProfiles navigation property.|
|[Add intuneBrandingProfiles](../api/devicemanagement-post-intunebrandingprofiles.md)|[intuneBrandingProfile](../resources/intunebrandingprofile.md)|Add intuneBrandingProfiles by posting to the intuneBrandingProfiles collection.|
|[List userPfxCertificates](../api/devicemanagement-list-userpfxcertificates.md)|[userPFXCertificate](../resources/userpfxcertificate.md) collection|Get the userPFXCertificates from the userPfxCertificates navigation property.|
|[Add userPfxCertificates](../api/devicemanagement-post-userpfxcertificates.md)|[userPFXCertificate](../resources/userpfxcertificate.md)|Add userPfxCertificates by posting to the userPfxCertificates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountMoveCompletionDateTime|DateTimeOffset||
|adminConsent|[adminConsent](../resources/adminconsent.md)||
|deviceComplianceReportSummarizationDateTime|DateTimeOffset||
|deviceProtectionOverview|[deviceProtectionOverview](../resources/deviceprotectionoverview.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|intuneAccountId|Guid||
|intuneBrand|[intuneBrand](../resources/intunebrand.md)||
|lastReportAggregationDateTime|DateTimeOffset||
|legacyPcManangementEnabled|Boolean||
|managedDeviceCleanupSettings|[managedDeviceCleanupSettings](../resources/manageddevicecleanupsettings.md)||
|maximumDepTokens|Int32||
|settings|[deviceManagementSettings](../resources/devicemanagementsettings.md)||
|subscriptions|Enumeration| Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.|
|subscriptionState|Enumeration| Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/windowsmalwareoverview.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|advancedThreatProtectionOnboardingStateSummary|[advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md)||
|androidDeviceOwnerEnrollmentProfiles|[androidDeviceOwnerEnrollmentProfile](../resources/androiddeviceownerenrollmentprofile.md) collection||
|androidForWorkAppConfigurationSchemas|[androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md) collection||
|androidForWorkEnrollmentProfiles|[androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) collection||
|androidForWorkSettings|[androidForWorkSettings](../resources/androidforworksettings.md)||
|androidManagedStoreAccountEnterpriseSettings|[androidManagedStoreAccountEnterpriseSettings](../resources/androidmanagedstoreaccountenterprisesettings.md)||
|androidManagedStoreAppConfigurationSchemas|[androidManagedStoreAppConfigurationSchema](../resources/androidmanagedstoreappconfigurationschema.md) collection||
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/applepushnotificationcertificate.md)||
|appleUserInitiatedEnrollmentProfiles|[appleUserInitiatedEnrollmentProfile](../resources/appleuserinitiatedenrollmentprofile.md) collection||
|auditEvents|[auditEvent](../resources/auditevent.md) collection||
|autopilotEvents|[deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) collection||
|cartToClassAssociations|[cartToClassAssociation](../resources/carttoclassassociation.md) collection||
|categories|[deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) collection||
|complianceManagementPartners|[complianceManagementPartner](../resources/compliancemanagementpartner.md) collection||
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md)||
|dataSharingConsents|[dataSharingConsent](../resources/datasharingconsent.md) collection||
|depOnboardingSettings|[depOnboardingSetting](../resources/deponboardingsetting.md) collection||
|derivedCredentials|[deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) collection||
|detectedApps|[detectedApp](../resources/detectedapp.md) collection||
|deviceCategories|[deviceCategory](../resources/devicecategory.md) collection||
|deviceCompliancePolicies|[deviceCompliancePolicy](../resources/devicecompliancepolicy.md) collection||
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/devicecompliancepolicydevicestatesummary.md)||
|deviceCompliancePolicySettingStateSummaries|[deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md) collection||
|deviceConfigurationConflictSummary|[deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md) collection||
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/deviceconfigurationdevicestatesummary.md)||
|deviceConfigurationRestrictedAppsViolations|[restrictedAppsViolation](../resources/restrictedappsviolation.md) collection||
|deviceConfigurations|[deviceConfiguration](../resources/deviceconfiguration.md) collection||
|deviceConfigurationsAllManagedDeviceCertificateStates|[managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md) collection||
|deviceConfigurationUserStateSummaries|[deviceConfigurationUserStateSummary](../resources/deviceconfigurationuserstatesummary.md)||
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md) collection||
|deviceHealthScripts|[deviceHealthScript](../resources/devicehealthscript.md) collection||
|deviceManagementPartners|[deviceManagementPartner](../resources/devicemanagementpartner.md) collection||
|deviceManagementScripts|[deviceManagementScript](../resources/devicemanagementscript.md) collection||
|deviceShellScripts|[deviceShellScript](../resources/deviceshellscript.md) collection||
|domainJoinConnectors|[deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md) collection||
|embeddedSIMActivationCodePools|[embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md) collection||
|exchangeConnectors|[deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) collection||
|exchangeOnPremisesPolicies|[deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md) collection||
|exchangeOnPremisesPolicy|[deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md)||
|groupPolicyCategories|[groupPolicyCategory](../resources/grouppolicycategory.md) collection||
|groupPolicyConfigurations|[groupPolicyConfiguration](../resources/grouppolicyconfiguration.md) collection||
|groupPolicyDefinitionFiles|[groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) collection||
|groupPolicyDefinitions|[groupPolicyDefinition](../resources/grouppolicydefinition.md) collection||
|groupPolicyMigrationReports|[groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) collection||
|groupPolicyObjectFiles|[groupPolicyObjectFile](../resources/grouppolicyobjectfile.md) collection||
|importedDeviceIdentities|[importedDeviceIdentity](../resources/importeddeviceidentity.md) collection||
|importedWindowsAutopilotDeviceIdentities|[importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md) collection||
|intents|[deviceManagementIntent](../resources/devicemanagementintent.md) collection||
|intuneBrandingProfiles|[intuneBrandingProfile](../resources/intunebrandingprofile.md) collection||
|iosUpdateStatuses|[iosUpdateDeviceStatus](../resources/iosupdatedevicestatus.md) collection||
|managedDeviceEncryptionStates|[managedDeviceEncryptionState](../resources/manageddeviceencryptionstate.md) collection||
|managedDeviceOverview|[managedDeviceOverview](../resources/manageddeviceoverview.md)||
|managedDevices|[managedDevice](../resources/manageddevice.md) collection||
|managementConditions|[managementCondition](../resources/managementcondition.md) collection||
|managementConditionStatements|[managementConditionStatement](../resources/managementconditionstatement.md) collection||
|mobileAppTroubleshootingEvents|[mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md) collection||
|mobileThreatDefenseConnectors|[mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) collection||
|ndesConnectors|[ndesConnector](../resources/ndesconnector.md) collection||
|notificationMessageTemplates|[notificationMessageTemplate](../resources/notificationmessagetemplate.md) collection||
|remoteActionAudits|[remoteActionAudit](../resources/remoteactionaudit.md) collection||
|remoteAssistancePartners|[remoteAssistancePartner](../resources/remoteassistancepartner.md) collection||
|reports|[deviceManagementReports](../resources/devicemanagementreports.md)||
|resourceOperations|[resourceOperation](../resources/resourceoperation.md) collection||
|roleAssignments|[deviceAndAppManagementRoleAssignment](../resources/deviceandappmanagementroleassignment.md) collection||
|roleDefinitions|[roleDefinition](../resources/roledefinition.md) collection||
|roleScopeTags|[roleScopeTag](../resources/rolescopetag.md) collection||
|settingDefinitions|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) collection||
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md)||
|telecomExpenseManagementPartners|[telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) collection||
|templates|[deviceManagementTemplate](../resources/devicemanagementtemplate.md) collection||
|termsAndConditions|[termsAndConditions](../resources/termsandconditions.md) collection||
|troubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md) collection||
|userExperienceAnalyticsBaselines|[userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md) collection||
|userExperienceAnalyticsCategories|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) collection||
|userExperienceAnalyticsDevicePerformance|[userExperienceAnalyticsDevicePerformance](../resources/userexperienceanalyticsdeviceperformance.md) collection||
|userExperienceAnalyticsDeviceStartupHistory|[userExperienceAnalyticsDeviceStartupHistory](../resources/userexperienceanalyticsdevicestartuphistory.md) collection||
|userExperienceAnalyticsDeviceStartupProcesses|[userExperienceAnalyticsDeviceStartupProcess](../resources/userexperienceanalyticsdevicestartupprocess.md) collection||
|userExperienceAnalyticsDeviceStartupProcessPerformance|[userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/userexperienceanalyticsdevicestartupprocessperformance.md) collection||
|userExperienceAnalyticsOverview|[userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md)||
|userExperienceAnalyticsRegressionSummary|[userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md)||
|userExperienceAnalyticsStartupScoreHistory|[userExperienceAnalyticsStartupScoreHistory](../resources/userexperienceanalyticsstartupscorehistory.md) collection||
|userPfxCertificates|[userPFXCertificate](../resources/userpfxcertificate.md) collection||
|windowsAutopilotDeploymentProfiles|[windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md) collection||
|windowsAutopilotDeviceIdentities|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) collection||
|windowsAutopilotSettings|[windowsAutopilotSettings](../resources/windowsautopilotsettings.md)||
|windowsFeatureUpdateProfiles|[windowsFeatureUpdateProfile](../resources/windowsfeatureupdateprofile.md) collection||
|windowsInformationProtectionAppLearningSummaries|[windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md) collection||
|windowsInformationProtectionNetworkLearningSummaries|[windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md) collection||
|windowsMalwareInformation|[windowsMalwareInformation](../resources/windowsmalwareinformation.md) collection||

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

