---
title: "remoteActionAudit resource type"
description: "Report of remote actions initiated on the devices belonging to a certain tenant."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# remoteActionAudit resource type


Namespace: microsoft.graph

Report of remote actions initiated on the devices belonging to a certain tenant.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List remoteActionAudits](../api/intune-devices-remoteactionaudit-list.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) collection|List properties and relationships of the [remoteActionAudit](../resources/remoteactionaudit.md) objects.|
|[Get remoteActionAudit](../api/intune-devices-remoteactionaudit-get.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.|
|[Create remoteActionAudit](../api/intune-devices-remoteactionaudit-create.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.|
|[Delete remoteActionAudit](../api/intune-devices-remoteactionaudit-delete.md)|None|Deletes a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).|
|[Update remoteActionAudit](../api/intune-devices-remoteactionaudit-update.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.|
|[List remoteActionAudits](../api/intune-devices-devicemanagement-list-remoteactionaudits.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) collection|Get the remoteActionAudits from the remoteActionAudits navigation property.|
|[Add remoteActionAudits](../api/intune-devices-devicemanagement-post-remoteactionaudits.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Add remoteActionAudits by posting to the remoteActionAudits collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|Enumeration|The action name. Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`, `rotateBitLockerKeys`, `rotateFileVaultKey`, `getFileVaultKey`, `setDeviceName`.|
|actionState|Enumeration|Action state. Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|deviceDisplayName|String|Intune device name.|
|deviceIMEI|String|IMEI of the device.|
|deviceOwnerUserPrincipalName|String|Upn of the device owner.|
|id|String| Inherited from [entity](../resources/entity.md)|
|initiatedByUserPrincipalName|String|User who initiated the device action, format is UPN.|
|managedDeviceId|String|Action target.|
|requestDateTime|DateTimeOffset|Time when the action was issued, given in UTC.|
|userName|String|\[deprecated\] Please use InitiatedByUserPrincipalName instead.|

## Relationships
None

## JSON Representation
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

