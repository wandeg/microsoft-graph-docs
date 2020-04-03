---
title: "mobileAppRelationshipState resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mobileAppRelationshipState resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceId|String||
|errorCode|Int32||
|installState|Enumeration| Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.|
|installStateDetail|Enumeration| Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.|
|sourceIds|String collection||
|targetDisplayName|String||
|targetId|String||
|targetLastSyncDateTime|DateTimeOffset||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppRelationshipState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppRelationshipState",
  "sourceIds": [
    "String"
  ],
  "targetId": "String",
  "targetDisplayName": "String",
  "deviceId": "String",
  "installState": "String",
  "installStateDetail": "String",
  "errorCode": 1024,
  "targetLastSyncDateTime": "String (timestamp)"
}
```

