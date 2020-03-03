---
title: "iosDeviceFeaturesConfiguration resource type"
description: "iOS Device Features Configuration Profile."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosDeviceFeaturesConfiguration resource type


Namespace: microsoft.graph

iOS Device Features Configuration Profile.


Inherits from [appleDeviceFeaturesConfigurationBase](../resources/appledevicefeaturesconfigurationbase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List iosDeviceFeaturesConfigurations](../api/iosdevicefeaturesconfiguration-list.md)|[iosDeviceFeaturesConfiguration](../resources/iosdevicefeaturesconfiguration.md) collection|List properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/iosdevicefeaturesconfiguration.md) objects.|
|[Get iosDeviceFeaturesConfiguration](../api/iosdevicefeaturesconfiguration-get.md)|[iosDeviceFeaturesConfiguration](../resources/iosdevicefeaturesconfiguration.md)|Read properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/iosdevicefeaturesconfiguration.md) object.|
|[Create iosDeviceFeaturesConfiguration](../api/iosdevicefeaturesconfiguration-create.md)|[iosDeviceFeaturesConfiguration](../resources/iosdevicefeaturesconfiguration.md)|Create a new [iosDeviceFeaturesConfiguration](../resources/iosdevicefeaturesconfiguration.md) object.|
|[Delete iosDeviceFeaturesConfiguration](../api/iosdevicefeaturesconfiguration-delete.md)|None|Deletes a [iosDeviceFeaturesConfiguration](../resources/iosdevicefeaturesconfiguration.md).|
|[Update iosDeviceFeaturesConfiguration](../api/iosdevicefeaturesconfiguration-update.md)|[iosDeviceFeaturesConfiguration](../resources/iosdevicefeaturesconfiguration.md)|Update the properties of a [iosDeviceFeaturesConfiguration](../resources/iosdevicefeaturesconfiguration.md) object.|
|[List groupAssignments](../api/iosdevicefeaturesconfiguration-list-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) collection|Get the deviceConfigurationGroupAssignments from the groupAssignments navigation property.|
|[Add groupAssignments](../api/iosdevicefeaturesconfiguration-post-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md)|Add groupAssignments by posting to the groupAssignments collection.|
|[List assignments](../api/iosdevicefeaturesconfiguration-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|Get the deviceConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/iosdevicefeaturesconfiguration-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/iosdevicefeaturesconfiguration-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Get the deviceConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/iosdevicefeaturesconfiguration-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/iosdevicefeaturesconfiguration-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Get the deviceConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/iosdevicefeaturesconfiguration-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[Get deviceConfigurationUserOverview](../api/deviceconfigurationuseroverview-get.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Read properties and relationships of the [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/iosdevicefeaturesconfiguration-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/iosdevicefeaturesconfiguration-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|
|[Get iosCertificateProfileBase](../api/ioscertificateprofilebase-get.md)|[iosCertificateProfileBase](../resources/ioscertificateprofilebase.md)|Read properties and relationships of the [iosCertificateProfileBase](../resources/ioscertificateprofilebase.md) object.|
|[Get iosCertificateProfileBase](../api/ioscertificateprofilebase-get.md)|[iosCertificateProfileBase](../resources/ioscertificateprofilebase.md)|Read properties and relationships of the [iosCertificateProfileBase](../resources/ioscertificateprofilebase.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|airPrintDestinations|[airPrintDestination](../resources/airprintdestination.md) collection|An array of AirPrint printers that should always be shown. This collection can contain a maximum of 500 elements. Inherited from [appleDeviceFeaturesConfigurationBase](../resources/appledevicefeaturesconfigurationbase.md)|
|assetTagTemplate|String|Asset tag information for the device, displayed on the login window and lock screen.|
|contentFilterSettings|[iosWebContentFilterBase](../resources/ioswebcontentfilterbase.md)|Gets or sets iOS Web Content Filter settings, supervised mode only|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/devicemanagementapplicabilityruledevicemode.md)|The device mode applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/devicemanagementapplicabilityruleosedition.md)|The OS edition applicability for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/devicemanagementapplicabilityruleosversion.md)|The OS version applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|homeScreenDockIcons|[iosHomeScreenItem](../resources/ioshomescreenitem.md) collection|A list of app and folders to appear on the Home Screen Dock. This collection can contain a maximum of 500 elements.|
|homeScreenPages|[iosHomeScreenPage](../resources/ioshomescreenpage.md) collection|A list of pages on the Home Screen. This collection can contain a maximum of 500 elements.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|lockScreenFootnote|String|A footnote displayed on the login window and lock screen. Available in iOS 9.3.1 and later.|
|notificationSettings|[iosNotificationSettings](../resources/iosnotificationsettings.md) collection|Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later). This collection can contain a maximum of 500 elements.|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|singleSignOnExtension|[singleSignOnExtension](../resources/singlesignonextension.md)|Gets or sets a single sign-on extension profile.|
|singleSignOnSettings|[iosSingleSignOnSettings](../resources/iossinglesignonsettings.md)|The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.|
|supportsScopeTags|Boolean|Indicates whether or not the underlying Device Configuration supports the assignment of scope tags. Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users. This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal. This property is read-only. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|wallpaperDisplayLocation|Enumeration|A wallpaper display location specifier. Possible values are: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.|
|wallpaperImage|[mimeContent](../resources/intune-apps-mimecontent.md)|A wallpaper image must be in either PNG or JPEG format. It requires a supervised device with iOS 8 or later version.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|The list of assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Device configuration installation status by device. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) collection|The list of group assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|identityCertificateForClientAuthentication|[iosCertificateProfileBase](../resources/ioscertificateprofilebase.md)|Identity Certificate for the renewal of Kerberos ticket used in single sign-on settings.|
|singleSignOnExtensionPkinitCertificate|[iosCertificateProfileBase](../resources/ioscertificateprofilebase.md)|PKINIT Certificate for the authentication with single sign-on extension settings.|
|userStatuses|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Device configuration installation status by user. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosDeviceFeaturesConfiguration",
  "baseType": "microsoft.graph.appleDeviceFeaturesConfigurationBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
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
  "assetTagTemplate": "String",
  "contentFilterSettings": {
    "@odata.type": "microsoft.graph.iosWebContentFilterBase"
  },
  "lockScreenFootnote": "String",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "bundleID": "String"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder"
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "appName": "String",
      "publisher": "String",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "String",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ],
  "singleSignOnSettings": {
    "@odata.type": "microsoft.graph.iosSingleSignOnSettings",
    "allowedAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "appStoreUrl": "String",
        "appId": "String"
      }
    ],
    "allowedUrls": [
      "String"
    ],
    "kerberosPrincipalName": "String",
    "kerberosRealm": "String"
  },
  "wallpaperDisplayLocation": "String",
  "wallpaperImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "singleSignOnExtension": {
    "@odata.type": "microsoft.graph.singleSignOnExtension"
  }
}
```

