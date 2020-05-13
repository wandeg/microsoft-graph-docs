---
title: "windowsWifiEnterpriseEAPConfiguration resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsWifiEnterpriseEAPConfiguration resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [windowsWifiConfiguration](../resources/windowswificonfiguration.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List rootCertificateForClientValidation](../api/windowswifienterpriseeapconfiguration-list-rootcertificateforclientvalidation.md)|[windows81TrustedRootCertificate](../resources/windows81trustedrootcertificate.md) collection|Get the windows81TrustedRootCertificate from the rootCertificateForClientValidation navigation property.|
|[Add rootCertificateForClientValidation](../api/windowswifienterpriseeapconfiguration-post-rootcertificateforclientvalidation.md)|[windows81TrustedRootCertificate](../resources/windows81trustedrootcertificate.md)|Add rootCertificateForClientValidation by posting to the rootCertificateForClientValidation collection.|
|[Remove rootCertificateForClientValidation](../api/windowswifienterpriseeapconfiguration-delete-rootcertificateforclientvalidation.md)|None|Remove a [windows81TrustedRootCertificate](../resources/windows81trustedrootcertificate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|authenticationMethod|wiFiAuthenticationMethod|**TODO: Add Description**. Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.|
|connectAutomatically|Boolean|**TODO: Add Description** Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md)|
|connectToPreferredNetwork|Boolean|**TODO: Add Description** Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Boolean|**TODO: Add Description** Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [deviceConfiguration](../resources/intune-deviceconfiguration.md)|
|description|String|**TODO: Add Description** Inherited from [deviceConfiguration](../resources/intune-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-devicemanagementapplicabilityruledevicemode.md)|**TODO: Add Description** Inherited from [deviceConfiguration](../resources/intune-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-devicemanagementapplicabilityruleosedition.md)|**TODO: Add Description** Inherited from [deviceConfiguration](../resources/intune-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-devicemanagementapplicabilityruleosversion.md)|**TODO: Add Description** Inherited from [deviceConfiguration](../resources/intune-deviceconfiguration.md)|
|displayName|String|**TODO: Add Description** Inherited from [deviceConfiguration](../resources/intune-deviceconfiguration.md)|
|eapType|eapType|**TODO: Add Description**. Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.|
|enablePairwiseMasterKeyCaching|Boolean|**TODO: Add Description**|
|enablePreAuthentication|Boolean|**TODO: Add Description**|
|forceFIPSCompliance|Boolean|**TODO: Add Description** Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|innerAuthenticationProtocolForEAPTTLS|nonEapAuthenticationMethodForEapTtlsType|**TODO: Add Description**. Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [deviceConfiguration](../resources/intune-deviceconfiguration.md)|
|maximumAuthenticationTimeoutInSeconds|Int32|**TODO: Add Description**|
|maximumNumberOfPairwiseMasterKeysInCache|Int32|**TODO: Add Description**|
|maximumPairwiseMasterKeyCacheTimeInMinutes|Int32|**TODO: Add Description**|
|maximumPreAuthenticationAttempts|Int32|**TODO: Add Description**|
|meteredConnectionLimit|meteredConnectionLimitType|**TODO: Add Description** Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md). Possible values are: `unrestricted`, `fixed`, `variable`.|
|networkName|String|**TODO: Add Description** Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md)|
|networkSingleSignOn|networkSingleSignOnType|**TODO: Add Description**. Possible values are: `disabled`, `prelogon`, `postlogon`.|
|outerIdentityPrivacyTemporaryValue|String|**TODO: Add Description**|
|preSharedKey|String|**TODO: Add Description** Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md)|
|promptForAdditionalAuthenticationCredentials|Boolean|**TODO: Add Description**|
|proxyAutomaticConfigurationUrl|String|**TODO: Add Description** Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md)|
|proxyManualAddress|String|**TODO: Add Description** Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md)|
|proxyManualPort|Int32|**TODO: Add Description** Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md)|
|proxySetting|wiFiProxySetting|**TODO: Add Description** Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md). Possible values are: `none`, `manual`, `automatic`.|
|roleScopeTagIds|String collection|**TODO: Add Description** Inherited from [deviceConfiguration](../resources/intune-deviceconfiguration.md)|
|ssid|String|**TODO: Add Description** Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md)|
|supportsScopeTags|Boolean|**TODO: Add Description** Inherited from [deviceConfiguration](../resources/intune-deviceconfiguration.md)|
|trustedServerCertificateNames|String collection|**TODO: Add Description**|
|version|Int32|**TODO: Add Description** Inherited from [deviceConfiguration](../resources/intune-deviceconfiguration.md)|
|wifiSecurityType|wiFiSecurityType|**TODO: Add Description** Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md). Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfigurationassignment.md) collection|**TODO: Add Description** Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-settingstatedevicesummary.md) collection|**TODO: Add Description** Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfigurationdevicestatus.md) collection|**TODO: Add Description** Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfigurationdeviceoverview.md)|**TODO: Add Description** Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfigurationgroupassignment.md) collection|**TODO: Add Description** Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|identityCertificateForClientAuthentication|[windowsCertificateProfileBase](../resources/windowscertificateprofilebase.md)|**TODO: Add Description**|
|rootCertificateForClientValidation|[windows81TrustedRootCertificate](../resources/windows81trustedrootcertificate.md)|**TODO: Add Description**|
|rootCertificatesForServerValidation|[windows81TrustedRootCertificate](../resources/windows81trustedrootcertificate.md) collection|**TODO: Add Description**|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfigurationuserstatus.md) collection|**TODO: Add Description** Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfigurationuseroverview.md)|**TODO: Add Description** Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "baseType": "microsoft.graph.windowsWifiConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": "Boolean",
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": "Integer",
  "preSharedKey": "String",
  "wifiSecurityType": "String",
  "meteredConnectionLimit": "String",
  "ssid": "String",
  "networkName": "String",
  "connectAutomatically": "Boolean",
  "connectToPreferredNetwork": "Boolean",
  "connectWhenNetworkNameIsHidden": "Boolean",
  "proxySetting": "String",
  "proxyManualAddress": "String",
  "proxyManualPort": "Integer",
  "proxyAutomaticConfigurationUrl": "String",
  "forceFIPSCompliance": "Boolean",
  "networkSingleSignOn": "String",
  "maximumAuthenticationTimeoutInSeconds": "Integer",
  "promptForAdditionalAuthenticationCredentials": "Boolean",
  "enablePairwiseMasterKeyCaching": "Boolean",
  "maximumPairwiseMasterKeyCacheTimeInMinutes": "Integer",
  "maximumNumberOfPairwiseMasterKeysInCache": "Integer",
  "enablePreAuthentication": "Boolean",
  "maximumPreAuthenticationAttempts": "Integer",
  "eapType": "String",
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEAPTTLS": "String",
  "outerIdentityPrivacyTemporaryValue": "String"
}
```

