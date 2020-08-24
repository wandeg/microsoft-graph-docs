---
title: "windowsProtectionState resource type"
description: "Device protection status entity."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# windowsProtectionState resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Device protection status entity.

## Methods

| Method                                                                                             | Return Type                                                           | Description                                                                        |
| :------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------- | :--------------------------------------------------------------------------------- |
| [List windowsProtectionState](../api/intune-windowsprotectionstate-list.md)                        | [windowsProtectionState](intune-windowsProtectionState.md) collection | List properties and relationships of a windowsProtectionState object.              |
| [Create windowsProtectionState](../api/intune-windowsprotectionstate-create.md)                    | [windowsProtectionState](intune-windowsProtectionState.md)            | Create a new windowsProtectionState object.                                        |
| [Get windowsProtectionState](../api/intune-windowsprotectionstate-get.md)                          | [windowsProtectionState](intune-windowsProtectionState.md)            | Read properties and relationships of a windowsProtectionState object.              |
| [Update windowsProtectionState](../api/intune-windowsprotectionstate-update.md)                    | [windowsProtectionState](intune-windowsProtectionState.md)            | Update the properties of a windowsProtectionState object.                          |
| [Delete windowsProtectionState](../api/intune-windowsprotectionstate-delete.md)                    |                                                                       | Delete a windowsProtectionState object.                                            |
| [List detectedMalwareState](../api/intune-windowsprotectionstate-list-detectedmalwarestate.md)     | windowsDeviceMalwareState                                             | Get the windowsDeviceMalwareState from a detectedMalwareState navigation property. |
| [Create detectedMalwareState](../api/intune-windowsprotectionstate-post-detectedmalwarestate.md)   | windowsDeviceMalwareState                                             | Create a new detectedMalwareState object.                                          |
| [Get detectedMalwareState](../api/intune-windowsprotectionstate-get-detectedmalwarestate.md)       | windowsDeviceMalwareState                                             | Read the properties and relationships of a windowsDeviceMalwareState object.       |
| [Update detectedMalwareState](../api/intune-windowsprotectionstate-update-detectedmalwarestate.md) | windowsDeviceMalwareState                                             | Update the properties of a detectedMalwareState object.                            |
| [Delete detectedMalwareState](../api/intune-windowsprotectionstate-delete-detectedmalwarestate.md) |                                                                       | Delete a windowsDeviceMalwareState object.                                         |

## Properties

| Property                       | Type           | Description                                                                                               |
| :----------------------------- | :------------- | :-------------------------------------------------------------------------------------------------------- |
| antiMalwareVersion             | String         | Current anti malware version                                                                              |
| deviceState                    | String         | Computer's state (like clean or pending full scan or pending reboot etc)                                  |
| engineVersion                  | String         | Current endpoint protection engine's version                                                              |
| fullScanOverdue                | Boolean        | Full scan overdue or not?                                                                                 |
| fullScanRequired               | Boolean        | Full scan required or not?                                                                                |
| id                             | String         | The unique Identifier for the device protection status object. This is device id of the device Read-only. |
| lastFullScanDateTime           | DateTimeOffset | Last quick scan datetime                                                                                  |
| lastFullScanSignatureVersion   | String         | Last full scan signature version                                                                          |
| lastQuickScanDateTime          | DateTimeOffset | Last quick scan datetime                                                                                  |
| lastQuickScanSignatureVersion  | String         | Last quick scan signature version                                                                         |
| lastReportedDateTime           | DateTimeOffset | Last device health status reported time                                                                   |
| malwareProtectionEnabled       | Boolean        | Anti malware is enabled or not                                                                            |
| networkInspectionSystemEnabled | Boolean        | Network inspection system enabled or not?                                                                 |
| quickScanOverdue               | Boolean        | Quick scan overdue or not?                                                                                |
| realTimeProtectionEnabled      | Boolean        | Real time protection is enabled or not?                                                                   |
| rebootRequired                 | Boolean        | Reboot required or not?                                                                                   |
| signatureUpdateOverdue         | Boolean        | Signature out of date or not?                                                                             |
| signatureVersion               | String         | Current malware definitions version                                                                       |

## Relationships

| Relationship         | Type                                                                              | Description         |
| :------------------- | :-------------------------------------------------------------------------------- | :------------------ |
| detectedMalwareState | [windowsDeviceMalwareState](../resources/windowsdevicemalwarestate.md) collection | Device malware list |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsProtectionState",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "antiMalwareVersion": "String",
  "deviceState": "clean | fullScanPending | rebootPending | manualStepsPending | offlineScanPending | critical",
  "engineVersion": "String",
  "fullScanOverdue": "Boolean",
  "fullScanRequired": "Boolean",
  "id": "String (identifier)",
  "lastFullScanDateTime": "DateTimeOffset",
  "lastFullScanSignatureVersion": "String",
  "lastQuickScanDateTime": "DateTimeOffset",
  "lastQuickScanSignatureVersion": "String",
  "lastReportedDateTime": "DateTimeOffset",
  "malwareProtectionEnabled": "Boolean",
  "networkInspectionSystemEnabled": "Boolean",
  "quickScanOverdue": "Boolean",
  "realTimeProtectionEnabled": "Boolean",
  "rebootRequired": "Boolean",
  "signatureUpdateOverdue": "Boolean",
  "signatureVersion": "String"
}
```