---
title: "win32LobApp resource type"
description: "Contains properties and inherited properties for Win32 apps."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# win32LobApp resource type


Namespace: microsoft.graph

Contains properties and inherited properties for Win32 apps.


Inherits from [mobileLobApp](../resources/mobilelobapp.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List win32LobApps](../api/win32lobapp-list.md)|[win32LobApp](../resources/win32lobapp.md) collection|List properties and relationships of the [win32LobApp](../resources/win32lobapp.md) objects.|
|[Get win32LobApp](../api/win32lobapp-get.md)|[win32LobApp](../resources/win32lobapp.md)|Read properties and relationships of the [win32LobApp](../resources/win32lobapp.md) object.|
|[Create win32LobApp](../api/win32lobapp-create.md)|[win32LobApp](../resources/win32lobapp.md)|Create a new [win32LobApp](../resources/win32lobapp.md) object.|
|[Delete win32LobApp](../api/win32lobapp-delete.md)|None|Deletes a [win32LobApp](../resources/win32lobapp.md).|
|[Update win32LobApp](../api/win32lobapp-update.md)|[win32LobApp](../resources/win32lobapp.md)|Update the properties of a [win32LobApp](../resources/win32lobapp.md) object.|
|[List categories](../api/win32lobapp-list-categories.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Create categories](../api/win32lobapp-post-categories.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Create categories by posting to the categories collection.|
|[List assignments](../api/win32lobapp-list-assignments.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection|Get the mobileAppAssignments from the assignments navigation property.|
|[Add assignments](../api/win32lobapp-post-assignments.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Add assignments by posting to the assignments collection.|
|[Get mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.|
|[List deviceStatuses](../api/win32lobapp-list-devicestatuses.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection|Get the mobileAppInstallStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/win32lobapp-post-devicestatuses.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/win32lobapp-list-userstatuses.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection|Get the userAppInstallStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/win32lobapp-post-userstatuses.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[List relationships](../api/win32lobapp-list-relationships.md)|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection|Get the mobileAppRelationships from the relationships navigation property.|
|[Add relationships](../api/win32lobapp-post-relationships.md)|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Add relationships by posting to the relationships collection.|
|[List contentVersions](../api/win32lobapp-list-contentversions.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection|Get the mobileAppContents from the contentVersions navigation property.|
|[Add contentVersions](../api/win32lobapp-post-contentversions.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Add contentVersions by posting to the contentVersions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicableArchitectures|Enumeration|The Windows architecture(s) for which this app can run on. Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.|
|committedContentVersion|String|The internal committed content version. Inherited from [mobileLobApp](../resources/mobilelobapp.md)|
|createdDateTime|DateTimeOffset|The date and time the app was created. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|dependentAppCount|Int32|The total number of dependencies the child app has. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|description|String|The description of the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|detectionRules|[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection|The detection rules to detect Win32 Line of Business (LoB) app.|
|developer|String|The developer of the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|displayName|String|The admin provided or imported title of the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|fileName|String|The name of the main Lob application file. Inherited from [mobileLobApp](../resources/mobilelobapp.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|informationUrl|String|The more information Url. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|installCommandLine|String|The command line to install this app|
|installExperience|[win32LobAppInstallExperience](../resources/intune-apps-win32lobappinstallexperience.md)|The install experience for this app.|
|isAssigned|Boolean|The value indicating whether the app is assigned to at least one group. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-apps-mimecontent.md)|The large icon, to be displayed in the app details and used for upload of the icon. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|minimumCpuSpeedInMHz|Int32|The value for the minimum CPU speed which is required to install this app.|
|minimumFreeDiskSpaceInMB|Int32|The value for the minimum free disk space which is required to install this app.|
|minimumMemoryInMB|Int32|The value for the minimum physical memory which is required to install this app.|
|minimumNumberOfProcessors|Int32|The value for the minimum number of processors which is required to install this app.|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/intune-apps-windowsminimumoperatingsystem.md)|The value for the minimum applicable operating system.|
|msiInformation|[win32LobAppMsiInformation](../resources/intune-apps-win32lobappmsiinformation.md)|The MSI details if this Win32 app is an MSI app.|
|notes|String|Notes for the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|owner|String|The owner of the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|publisher|String|The publisher of the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|publishingState|Enumeration|The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md). Possible values are: `notPublished`, `processing`, `published`.|
|requirementRules|[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection|The requirement rules to detect Win32 Line of Business (LoB) app.|
|returnCodes|[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection|The return codes for post installation behavior.|
|roleScopeTagIds|String collection|List of scope tag ids for this mobile app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|setupFilePath|String|The relative path of the setup file in the encrypted Win32LobApp package.|
|size|Int64|The total size, including all uploaded files. Inherited from [mobileLobApp](../resources/mobilelobapp.md)|
|uninstallCommandLine|String|The command line to uninstall this app|
|uploadState|Int32|The upload state. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection|The list of group assignments for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection|The list of categories for this app. Inherited from [mobileApp](../resources/mobileapp.md)|
|contentVersions|[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection|The list of content versions for this app. Inherited from [mobileLobApp](../resources/mobilelobapp.md)|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection|The list of installation states for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Mobile App Install Summary. Inherited from [mobileApp](../resources/mobileapp.md)|
|relationships|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection|List of relationships for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection|The list of installation states for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.win32LobApp",
  "baseType": "microsoft.graph.mobileLobApp",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "uploadState": 1024,
  "publishingState": "String",
  "isAssigned": true,
  "roleScopeTagIds": [
    "String"
  ],
  "dependentAppCount": 1024,
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "installCommandLine": "String",
  "uninstallCommandLine": "String",
  "applicableArchitectures": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "minimumFreeDiskSpaceInMB": 1024,
  "minimumMemoryInMB": 1024,
  "minimumNumberOfProcessors": 1024,
  "minimumCpuSpeedInMHz": 1024,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "String",
      "valueName": "String",
      "detectionType": "String",
      "operator": "String",
      "detectionValue": "String"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "String",
    "deviceRestartBehavior": "String"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 1024,
      "type": "String"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "String",
    "productVersion": "String",
    "upgradeCode": "String",
    "requiresReboot": true,
    "packageType": "String",
    "productName": "String"
  },
  "setupFilePath": "String"
}
```

