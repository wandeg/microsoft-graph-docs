---
title: "mobileAppInstallStatus resource type"
description: "Contains properties for the installation state of a mobile app for a device."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mobileAppInstallStatus resource type


Namespace: microsoft.graph

Contains properties for the installation state of a mobile app for a device.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get mobileAppInstallStatus](../api/mobileappinstallstatus-get.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md)|Read the properties and relationships of a [mobileAppInstallStatus](../resources/mobileappinstallstatus.md) object.|
|[Update mobileAppInstallStatus](../api/mobileappinstallstatus-update.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md)|Update the properties of a [mobileAppInstallStatus](../resources/mobileappinstallstatus.md) object.|
|[List app](../api/mobileappinstallstatus-list-app.md)|[mobileApp](../resources/mobileapp.md) collection|Get the mobileApps from the app navigation property.|
|[Add app](../api/mobileappinstallstatus-post-app.md)|[mobileApp](../resources/mobileapp.md)|Add app by posting to the app collection.|
|[Remove app](../api/mobileappinstallstatus-delete-app.md)|None|Remove an [mobileApp](../resources/mobileapp.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceId|String|Device ID|
|deviceName|String|Device name|
|displayVersion|String|Human readable version of the application|
|errorCode|Int32|The error code for install or uninstall failures.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|installState|resultantAppState|The install state of the app. Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.|
|installStateDetail|resultantAppStateDetail|The install state detail of the app. Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.|
|lastSyncDateTime|DateTimeOffset|Last sync date time|
|mobileAppInstallStatusValue|resultantAppState|The install state of the app. Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.|
|osDescription|String|OS Description|
|osVersion|String|OS Version|
|userName|String|Device User Name|
|userPrincipalName|String|User Principal Name|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|app|[mobileApp](../resources/mobileapp.md)|The navigation link to the mobile app.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallStatus",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "mobileAppInstallStatusValue": "String",
  "installState": "String",
  "installStateDetail": "String",
  "errorCode": 1024,
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "displayVersion": "String"
}
```

