---
title: "macOSDeviceFeaturesConfiguration resource type"
description: "MacOS device features configuration profile."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# macOSDeviceFeaturesConfiguration resource type


Namespace: microsoft.graph

MacOS device features configuration profile.


Inherits from [appleDeviceFeaturesConfigurationBase](../resources/appledevicefeaturesconfigurationbase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List macOSDeviceFeaturesConfigurations](../api/macosdevicefeaturesconfiguration-list.md)|[macOSDeviceFeaturesConfiguration](../resources/macosdevicefeaturesconfiguration.md) collection|List properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/macosdevicefeaturesconfiguration.md) objects.|
|[Get macOSDeviceFeaturesConfiguration](../api/macosdevicefeaturesconfiguration-get.md)|[macOSDeviceFeaturesConfiguration](../resources/macosdevicefeaturesconfiguration.md)|Read properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/macosdevicefeaturesconfiguration.md) object.|
|[Create macOSDeviceFeaturesConfiguration](../api/macosdevicefeaturesconfiguration-create.md)|[macOSDeviceFeaturesConfiguration](../resources/macosdevicefeaturesconfiguration.md)|Create a new [macOSDeviceFeaturesConfiguration](../resources/macosdevicefeaturesconfiguration.md) object.|
|[Delete macOSDeviceFeaturesConfiguration](../api/macosdevicefeaturesconfiguration-delete.md)|None|Deletes a [macOSDeviceFeaturesConfiguration](../resources/macosdevicefeaturesconfiguration.md).|
|[Update macOSDeviceFeaturesConfiguration](../api/macosdevicefeaturesconfiguration-update.md)|[macOSDeviceFeaturesConfiguration](../resources/macosdevicefeaturesconfiguration.md)|Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/macosdevicefeaturesconfiguration.md) object.|
|[List groupAssignments](../api/macosdevicefeaturesconfiguration-list-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) collection|Get the deviceConfigurationGroupAssignments from the groupAssignments navigation property.|
|[Add groupAssignments](../api/macosdevicefeaturesconfiguration-post-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md)|Add groupAssignments by posting to the groupAssignments collection.|
|[List assignments](../api/macosdevicefeaturesconfiguration-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|Get the deviceConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/macosdevicefeaturesconfiguration-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/macosdevicefeaturesconfiguration-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Get the deviceConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/macosdevicefeaturesconfiguration-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/macosdevicefeaturesconfiguration-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Get the deviceConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/macosdevicefeaturesconfiguration-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[Get deviceConfigurationUserOverview](../api/deviceconfigurationuseroverview-get.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Read properties and relationships of the [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/macosdevicefeaturesconfiguration-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/macosdevicefeaturesconfiguration-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|
|[Get macOSCertificateProfileBase](../api/macoscertificateprofilebase-get.md)|[macOSCertificateProfileBase](../resources/macoscertificateprofilebase.md)|Read properties and relationships of the [macOSCertificateProfileBase](../resources/macoscertificateprofilebase.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|adminShowHostInfo|Boolean|Whether to show admin host information on the login window.|
|airPrintDestinations|[airPrintDestination](../resources/airprintdestination.md) collection|An array of AirPrint printers that should always be shown. This collection can contain a maximum of 500 elements. Inherited from [appleDeviceFeaturesConfigurationBase](../resources/appledevicefeaturesconfigurationbase.md)|
|associatedDomains|[keyValuePair](../resources/keyvaluepair.md) collection|Gets or sets a list that maps apps to their associated domains. The key should match the app's ID, and the value should be a string in the form of "service:domain" where domain is a fully qualified hostname (e.g. webcredentials:example.com). This collection can contain a maximum of 500 elements.|
|authorizedUsersListHidden|Boolean|Whether to show the name and password dialog or a list of users on the login window.|
|authorizedUsersListHideAdminUsers|Boolean|Whether to hide admin users in the authorized users list on the login window.|
|authorizedUsersListHideLocalUsers|Boolean|Whether to show only network and system users in the authorized users list on the login window.|
|authorizedUsersListHideMobileAccounts|Boolean|Whether to hide mobile users in the authorized users list on the login window.|
|authorizedUsersListIncludeNetworkUsers|Boolean|Whether to show network users in the authorized users list on the login window.|
|authorizedUsersListShowOtherManagedUsers|Boolean|Whether to show other users in the authorized users list on the login window.|
|autoLaunchItems|[macOSLaunchItem](../resources/macoslaunchitem.md) collection|List of applications, files, folders, and other items to launch when the user logs in. This collection can contain a maximum of 500 elements.|
|consoleAccessDisabled|Boolean|Whether the Other user will disregard use of the `>console> special user name.|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/devicemanagementapplicabilityruledevicemode.md)|The device mode applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/devicemanagementapplicabilityruleosedition.md)|The OS edition applicability for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/devicemanagementapplicabilityruleosversion.md)|The OS version applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|loginWindowText|String|Custom text to be displayed on the login window.|
|logOutDisabledWhileLoggedIn|Boolean|Whether the Log Out menu item on the login window will be disabled while the user is logged in.|
|powerOffDisabledWhileLoggedIn|Boolean|Whether the Power Off menu item on the login window will be disabled while the user is logged in.|
|restartDisabled|Boolean|Whether to hide the Restart button item on the login window.|
|restartDisabledWhileLoggedIn|Boolean|Whether the Restart menu item on the login window will be disabled while the user is logged in.|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|screenLockDisableImmediate|Boolean|Whether to disable the immediate screen lock functions.|
|shutDownDisabled|Boolean|Whether to hide the Shut Down button item on the login window.|
|shutDownDisabledWhileLoggedIn|Boolean|Whether the Shut Down menu item on the login window will be disabled while the user is logged in.|
|singleSignOnExtension|[singleSignOnExtension](../resources/singlesignonextension.md)|Gets or sets a single sign-on extension profile.|
|sleepDisabled|Boolean|Whether to hide the Sleep menu item on the login window.|
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
|singleSignOnExtensionPkinitCertificate|[macOSCertificateProfileBase](../resources/macoscertificateprofilebase.md)|PKINIT Certificate for the authentication with single sign-on extensions.|
|userStatuses|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Device configuration installation status by user. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSDeviceFeaturesConfiguration",
  "baseType": "microsoft.graph.appleDeviceFeaturesConfigurationBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
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
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "String",
      "resourcePath": "String",
      "port": 1024,
      "forceTls": true
    }
  ],
  "autoLaunchItems": [
    {
      "@odata.type": "microsoft.graph.macOSLaunchItem",
      "path": "String",
      "hide": true
    }
  ],
  "adminShowHostInfo": true,
  "loginWindowText": "String",
  "authorizedUsersListHidden": true,
  "authorizedUsersListHideLocalUsers": true,
  "authorizedUsersListHideMobileAccounts": true,
  "authorizedUsersListIncludeNetworkUsers": true,
  "authorizedUsersListHideAdminUsers": true,
  "authorizedUsersListShowOtherManagedUsers": true,
  "shutDownDisabled": true,
  "restartDisabled": true,
  "sleepDisabled": true,
  "consoleAccessDisabled": true,
  "shutDownDisabledWhileLoggedIn": true,
  "restartDisabledWhileLoggedIn": true,
  "powerOffDisabledWhileLoggedIn": true,
  "logOutDisabledWhileLoggedIn": true,
  "screenLockDisableImmediate": true,
  "associatedDomains": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "value": "String"
    }
  ],
  "singleSignOnExtension": {
    "@odata.type": "microsoft.graph.singleSignOnExtension"
  }
}
```

