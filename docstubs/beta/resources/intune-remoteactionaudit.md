---
title: "remoteActionAudit resource type"
description: "Report of remote actions initiated on the devices belonging to a certain tenant."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# remoteActionAudit resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Report of remote actions initiated on the devices belonging to a certain tenant.

## Methods

| Method                                                                | Return Type                                                 | Description                                                      |
| :-------------------------------------------------------------------- | :---------------------------------------------------------- | :--------------------------------------------------------------- |
| [List remoteActionAudit](../api/intune-remoteactionaudit-list.md)     | [remoteActionAudit](intune-remoteActionAudit.md) collection | List properties and relationships of a remoteActionAudit object. |
| [Create remoteActionAudit](../api/intune-remoteactionaudit-create.md) | [remoteActionAudit](intune-remoteActionAudit.md)            | Create a new remoteActionAudit object.                           |
| [Get remoteActionAudit](../api/intune-remoteactionaudit-get.md)       | [remoteActionAudit](intune-remoteActionAudit.md)            | Read properties and relationships of a remoteActionAudit object. |
| [Update remoteActionAudit](../api/intune-remoteactionaudit-update.md) | [remoteActionAudit](intune-remoteActionAudit.md)            | Update the properties of a remoteActionAudit object.             |
| [Delete remoteActionAudit](../api/intune-remoteactionaudit-delete.md) |                                                             | Delete a remoteActionAudit object.                               |

## Properties

| Property                     | Type           | Description                                                   |
| :--------------------------- | :------------- | :------------------------------------------------------------ |
| action                       | String         | The action name.                                              |
| actionState                  | String         | Action state.                                                 |
| deviceDisplayName            | String         | Intune device name.                                           |
| deviceIMEI                   | String         | IMEI of the device.                                           |
| deviceOwnerUserPrincipalName | String         | Upn of the device owner.                                      |
| id                           | String         | Report Id. Read-only.                                         |
| initiatedByUserPrincipalName | String         | User who initiated the device action, format is UPN.          |
| managedDeviceId              | String         | Action target.                                                |
| requestDateTime              | DateTimeOffset | Time when the action was issued, given in UTC.                |
| userName                     | String         | [deprecated] Please use InitiatedByUserPrincipalName instead. |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteActionAudit",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "action": "unknown | factoryReset | removeCompanyData | resetPasscode | remoteLock | enableLostMode | disableLostMode | locateDevice | rebootNow | recoverPasscode | cleanWindowsDevice | logoutSharedAppleDeviceActiveUser | quickScan | fullScan | windowsDefenderUpdateSignatures | factoryResetKeepEnrollmentData | updateDeviceAccount | automaticRedeployment | shutDown | rotateBitLockerKeys | rotateFileVaultKey | getFileVaultKey | setDeviceName",
  "actionState": "none | pending | canceled | active | done | failed | notSupported",
  "deviceDisplayName": "String",
  "deviceIMEI": "String",
  "deviceOwnerUserPrincipalName": "String",
  "id": "String (identifier)",
  "initiatedByUserPrincipalName": "String",
  "managedDeviceId": "String",
  "requestDateTime": "DateTimeOffset",
  "userName": "String"
}
```