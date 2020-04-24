---
title: "remoteActionAudit resource type"
description: "Report of remote actions initiated on the devices belonging to a certain tenant."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# remoteActionAudit resource type


Namespace: microsoft.graph

Report of remote actions initiated on the devices belonging to a certain tenant.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get remoteActionAudit](../api/remoteactionaudit-get.md)|[remoteActionAudit](../resources/remoteactionaudit.md)|Read the properties and relationships of a [remoteActionAudit](../resources/remoteactionaudit.md) object.|
|[Update remoteActionAudit](../api/remoteactionaudit-update.md)|[remoteActionAudit](../resources/remoteactionaudit.md)|Update the properties of a [remoteActionAudit](../resources/remoteactionaudit.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|remoteAction|The action name. Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`, `rotateBitLockerKeys`, `rotateFileVaultKey`, `getFileVaultKey`, `setDeviceName`.|
|actionState|actionState|Action state. Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|deviceDisplayName|String|Intune device name.|
|deviceIMEI|String|IMEI of the device.|
|deviceOwnerUserPrincipalName|String|Upn of the device owner.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|initiatedByUserPrincipalName|String|User who initiated the device action, format is UPN.|
|managedDeviceId|String|Action target.|
|requestDateTime|DateTimeOffset|Time when the action was issued, given in UTC.|
|userName|String|\[deprecated\] Please use InitiatedByUserPrincipalName instead.|

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

