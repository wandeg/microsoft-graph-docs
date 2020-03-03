---
title: "windowsProtectionState resource type"
description: "Device protection status entity."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsProtectionState resource type


Namespace: microsoft.graph

Device protection status entity.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windowsProtectionStates](../api/intune-devices-windowsprotectionstate-list.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) collection|List properties and relationships of the [windowsProtectionState](../resources/windowsprotectionstate.md) objects.|
|[Get windowsProtectionState](../api/intune-devices-windowsprotectionstate-get.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.|
|[Create windowsProtectionState](../api/intune-devices-windowsprotectionstate-create.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Create a new [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.|
|[Delete windowsProtectionState](../api/intune-devices-windowsprotectionstate-delete.md)|None|Deletes a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).|
|[Update windowsProtectionState](../api/intune-devices-windowsprotectionstate-update.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.|
|[List detectedMalwareState](../api/intune-devices-windowsprotectionstate-list-detectedmalwarestate.md)|[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection|Get the windowsDeviceMalwareStates from the detectedMalwareState navigation property.|
|[Add detectedMalwareState](../api/intune-devices-windowsprotectionstate-post-detectedmalwarestate.md)|[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)|Add detectedMalwareState by posting to the detectedMalwareState collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|antiMalwareVersion|String|Current anti malware version|
|deviceState|Enumeration|Computer's state (like clean or pending full scan or pending reboot etc). Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|engineVersion|String|Current endpoint protection engine's version|
|fullScanOverdue|Boolean|Full scan overdue or not?|
|fullScanRequired|Boolean|Full scan required or not?|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastFullScanDateTime|DateTimeOffset|Last quick scan datetime|
|lastFullScanSignatureVersion|String|Last full scan signature version|
|lastQuickScanDateTime|DateTimeOffset|Last quick scan datetime|
|lastQuickScanSignatureVersion|String|Last quick scan signature version|
|lastReportedDateTime|DateTimeOffset|Last device health status reported time|
|malwareProtectionEnabled|Boolean|Anti malware is enabled or not|
|networkInspectionSystemEnabled|Boolean|Network inspection system enabled or not?|
|quickScanOverdue|Boolean|Quick scan overdue or not?|
|realTimeProtectionEnabled|Boolean|Real time protection is enabled or not?|
|rebootRequired|Boolean|Reboot required or not?|
|signatureUpdateOverdue|Boolean|Signature out of date or not?|
|signatureVersion|String|Current malware definitions version|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|detectedMalwareState|[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection|Device malware list|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsProtectionState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "String (identifier)",
  "malwareProtectionEnabled": true,
  "deviceState": "String",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "String",
  "signatureVersion": "String",
  "antiMalwareVersion": "String",
  "lastQuickScanDateTime": "String (timestamp)",
  "lastFullScanDateTime": "String (timestamp)",
  "lastQuickScanSignatureVersion": "String",
  "lastFullScanSignatureVersion": "String",
  "lastReportedDateTime": "String (timestamp)"
}
```

