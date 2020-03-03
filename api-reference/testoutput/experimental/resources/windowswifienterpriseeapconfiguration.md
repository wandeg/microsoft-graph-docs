---
title: "windowsWifiEnterpriseEAPConfiguration resource type"
description: "This entity provides descriptions of the declared methods, properties and relationships exposed by the Wifi CSP."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsWifiEnterpriseEAPConfiguration resource type


Namespace: microsoft.graph

This entity provides descriptions of the declared methods, properties and relationships exposed by the Wifi CSP.


Inherits from [windowsWifiConfiguration](../resources/windowswificonfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windowsWifiEnterpriseEAPConfigurations](../api/windowswifienterpriseeapconfiguration-list.md)|[windowsWifiEnterpriseEAPConfiguration](../resources/windowswifienterpriseeapconfiguration.md) collection|List properties and relationships of the [windowsWifiEnterpriseEAPConfiguration](../resources/windowswifienterpriseeapconfiguration.md) objects.|
|[Get windowsWifiEnterpriseEAPConfiguration](../api/windowswifienterpriseeapconfiguration-get.md)|[windowsWifiEnterpriseEAPConfiguration](../resources/windowswifienterpriseeapconfiguration.md)|Read properties and relationships of the [windowsWifiEnterpriseEAPConfiguration](../resources/windowswifienterpriseeapconfiguration.md) object.|
|[Create windowsWifiEnterpriseEAPConfiguration](../api/windowswifienterpriseeapconfiguration-create.md)|[windowsWifiEnterpriseEAPConfiguration](../resources/windowswifienterpriseeapconfiguration.md)|Create a new [windowsWifiEnterpriseEAPConfiguration](../resources/windowswifienterpriseeapconfiguration.md) object.|
|[Delete windowsWifiEnterpriseEAPConfiguration](../api/windowswifienterpriseeapconfiguration-delete.md)|None|Deletes a [windowsWifiEnterpriseEAPConfiguration](../resources/windowswifienterpriseeapconfiguration.md).|
|[Update windowsWifiEnterpriseEAPConfiguration](../api/windowswifienterpriseeapconfiguration-update.md)|[windowsWifiEnterpriseEAPConfiguration](../resources/windowswifienterpriseeapconfiguration.md)|Update the properties of a [windowsWifiEnterpriseEAPConfiguration](../resources/windowswifienterpriseeapconfiguration.md) object.|
|[List groupAssignments](../api/windowswifienterpriseeapconfiguration-list-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) collection|Get the deviceConfigurationGroupAssignments from the groupAssignments navigation property.|
|[Add groupAssignments](../api/windowswifienterpriseeapconfiguration-post-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md)|Add groupAssignments by posting to the groupAssignments collection.|
|[List assignments](../api/windowswifienterpriseeapconfiguration-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|Get the deviceConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/windowswifienterpriseeapconfiguration-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/windowswifienterpriseeapconfiguration-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Get the deviceConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/windowswifienterpriseeapconfiguration-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/windowswifienterpriseeapconfiguration-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Get the deviceConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/windowswifienterpriseeapconfiguration-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[Get deviceConfigurationUserOverview](../api/deviceconfigurationuseroverview-get.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Read properties and relationships of the [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/windowswifienterpriseeapconfiguration-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/windowswifienterpriseeapconfiguration-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|
|[List rootCertificatesForServerValidation](../api/windowswifienterpriseeapconfiguration-list-rootcertificatesforservervalidation.md)|[windows81TrustedRootCertificate](../resources/windows81trustedrootcertificate.md) collection|Get the windows81TrustedRootCertificates from the rootCertificatesForServerValidation navigation property.|
|[Create rootCertificatesForServerValidation](../api/windowswifienterpriseeapconfiguration-post-rootcertificatesforservervalidation.md)|[windows81TrustedRootCertificate](../resources/windows81trustedrootcertificate.md)|Create rootCertificatesForServerValidation by posting to the rootCertificatesForServerValidation collection.|
|[Get windowsCertificateProfileBase](../api/windowscertificateprofilebase-get.md)|[windowsCertificateProfileBase](../resources/windowscertificateprofilebase.md)|Read properties and relationships of the [windowsCertificateProfileBase](../resources/windowscertificateprofilebase.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|authenticationMethod|Enumeration|Specify the authentication method. Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.|
|connectAutomatically|Boolean|Specify whether the wifi connection should connect automatically when in range. Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md)|
|connectToPreferredNetwork|Boolean|Specify whether the wifi connection should connect to more preferred networks when already connected to this one.  Requires ConnectAutomatically to be true. Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Boolean|Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting. Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/devicemanagementapplicabilityruledevicemode.md)|The device mode applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/devicemanagementapplicabilityruleosedition.md)|The OS edition applicability for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/devicemanagementapplicabilityruleosversion.md)|The OS version applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|eapType|Enumeration|Extensible Authentication Protocol (EAP). Indicates the type of EAP protocol set on the Wi-Fi endpoint (router). Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.|
|enablePairwiseMasterKeyCaching|Boolean|Specify whether the wifi connection should enable pairwise master key caching.|
|enablePreAuthentication|Boolean|Specify whether pre-authentication should be enabled.|
|forceFIPSCompliance|Boolean|Specify whether to force FIPS compliance. Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|innerAuthenticationProtocolForEAPTTLS|Enumeration|Specify inner authentication protocol for EAP TTLS. Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|maximumAuthenticationTimeoutInSeconds|Int32|Specify maximum authentication timeout (in seconds).  Valid range: 1-120|
|maximumNumberOfPairwiseMasterKeysInCache|Int32|Specify maximum number of pairwise master keys in cache.  Valid range: 1-255|
|maximumPairwiseMasterKeyCacheTimeInMinutes|Int32|Specify maximum pairwise master key cache time (in minutes).  Valid range: 5-1440|
|maximumPreAuthenticationAttempts|Int32|Specify maximum pre-authentication attempts.  Valid range: 1-16|
|meteredConnectionLimit|Enumeration|Specify the metered connection limit type for the wifi connection. Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md). Possible values are: `unrestricted`, `fixed`, `variable`.|
|networkName|String|Specify the network configuration name. Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md)|
|networkSingleSignOn|Enumeration|Specify the network single sign on type. Possible values are: `disabled`, `prelogon`, `postlogon`.|
|outerIdentityPrivacyTemporaryValue|String|Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.|
|preSharedKey|String|This is the pre-shared key for WPA Personal Wi-Fi network. Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md)|
|promptForAdditionalAuthenticationCredentials|Boolean|Specify whether the wifi connection should prompt for additional authentication credentials.|
|proxyAutomaticConfigurationUrl|String|Specify the URL for the proxy server configuration script. Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md)|
|proxyManualAddress|String|Specify the IP address for the proxy server. Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md)|
|proxyManualPort|Int32|Specify the port for the proxy server. Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md)|
|proxySetting|Enumeration|Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md). Possible values are: `none`, `manual`, `automatic`.|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|ssid|String|Specify the SSID of the wifi connection. Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md)|
|supportsScopeTags|Boolean|Indicates whether or not the underlying Device Configuration supports the assignment of scope tags. Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users. This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal. This property is read-only. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|trustedServerCertificateNames|String collection|Specify trusted server certificate names.|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|wifiSecurityType|Enumeration|Specify the Wifi Security Type. Inherited from [windowsWifiConfiguration](../resources/windowswificonfiguration.md). Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|The list of assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Device configuration installation status by device. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) collection|The list of group assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|identityCertificateForClientAuthentication|[windowsCertificateProfileBase](../resources/windowscertificateprofilebase.md)|Specify identity certificate for client authentication.|
|rootCertificatesForServerValidation|[windows81TrustedRootCertificate](../resources/windows81trustedrootcertificate.md) collection|Specify root certificate for server validation.|
|userStatuses|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Device configuration installation status by user. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|

## JSON Representation
Here is a JSON representation of the resource.
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
  "supportsScopeTags": true,
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
  "version": 1024,
  "preSharedKey": "String",
  "wifiSecurityType": "String",
  "meteredConnectionLimit": "String",
  "ssid": "String",
  "networkName": "String",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "String",
  "proxyManualAddress": "String",
  "proxyManualPort": 1024,
  "proxyAutomaticConfigurationUrl": "String",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "String",
  "maximumAuthenticationTimeoutInSeconds": 1024,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 1024,
  "maximumNumberOfPairwiseMasterKeysInCache": 1024,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 1024,
  "eapType": "String",
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEAPTTLS": "String",
  "outerIdentityPrivacyTemporaryValue": "String"
}
```

