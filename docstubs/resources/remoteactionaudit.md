---
title: "remoteActionAudit resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# remoteActionAudit resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get remoteActionAudit](../api/remoteactionaudit-get.md)|[remoteActionAudit](../resources/remoteactionaudit.md)|Read properties and relationships of the [remoteActionAudit](../resources/remoteactionaudit.md) object.|
|[Update remoteActionAudit](../api/remoteactionaudit-update.md)|[remoteActionAudit](../resources/remoteactionaudit.md)|Update the properties of a [remoteActionAudit](../resources/remoteactionaudit.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|Enumeration| Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`, `rotateBitLockerKeys`, `rotateFileVaultKey`, `getFileVaultKey`, `setDeviceName`.|
|actionState|Enumeration| Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|deviceDisplayName|String||
|deviceIMEI|String||
|deviceOwnerUserPrincipalName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|initiatedByUserPrincipalName|String||
|managedDeviceId|String||
|requestDateTime|DateTimeOffset||
|userName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteActionAudit",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "initiatedByUserPrincipalName": "String",
  "action": "String",
  "requestDateTime": "String (timestamp)",
  "deviceOwnerUserPrincipalName": "String",
  "deviceIMEI": "String",
  "actionState": "String",
  "managedDeviceId": "String"
}
```

