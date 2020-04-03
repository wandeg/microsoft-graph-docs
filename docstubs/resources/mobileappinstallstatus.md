---
title: "mobileAppInstallStatus resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mobileAppInstallStatus resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get mobileAppInstallStatus](../api/mobileappinstallstatus-get.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md)|Read properties and relationships of the [mobileAppInstallStatus](../resources/mobileappinstallstatus.md) object.|
|[Update mobileAppInstallStatus](../api/mobileappinstallstatus-update.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md)|Update the properties of a [mobileAppInstallStatus](../resources/mobileappinstallstatus.md) object.|
|[Get mobileApp](../api/mobileapp-get.md)|[mobileApp](../resources/mobileapp.md)|Read properties and relationships of the [mobileApp](../resources/mobileapp.md) object.|
|[List deviceStatuses](../api/mobileapp-list-devicestatuses.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md) collection|Get the mobileAppInstallStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/mobileapp-post-devicestatuses.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceId|String||
|deviceName|String||
|displayVersion|String||
|errorCode|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|
|installState|Enumeration| Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.|
|installStateDetail|Enumeration| Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.|
|lastSyncDateTime|DateTimeOffset||
|mobileAppInstallStatusValue|Enumeration| Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.|
|osDescription|String||
|osVersion|String||
|userName|String||
|userPrincipalName|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|app|[mobileApp](../resources/mobileapp.md)||

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

