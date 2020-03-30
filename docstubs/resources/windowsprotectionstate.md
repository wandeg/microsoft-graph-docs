---
title: "windowsProtectionState resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsProtectionState resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsProtectionState](../api/windowsprotectionstate-get.md)|[windowsProtectionState](../resources/windowsprotectionstate.md)|Read properties and relationships of the [windowsProtectionState](../resources/windowsprotectionstate.md) object.|
|[Update windowsProtectionState](../api/windowsprotectionstate-update.md)|[windowsProtectionState](../resources/windowsprotectionstate.md)|Update the properties of a [windowsProtectionState](../resources/windowsprotectionstate.md) object.|
|[List detectedMalwareState](../api/windowsprotectionstate-list-detectedmalwarestate.md)|[windowsDeviceMalwareState](../resources/windowsdevicemalwarestate.md) collection|Get the windowsDeviceMalwareStates from the detectedMalwareState navigation property.|
|[Add detectedMalwareState](../api/windowsprotectionstate-post-detectedmalwarestate.md)|[windowsDeviceMalwareState](../resources/windowsdevicemalwarestate.md)|Add detectedMalwareState by posting to the detectedMalwareState collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|antiMalwareVersion|String||
|deviceState|Enumeration| Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|engineVersion|String||
|fullScanOverdue|Boolean||
|fullScanRequired|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastFullScanDateTime|DateTimeOffset||
|lastFullScanSignatureVersion|String||
|lastQuickScanDateTime|DateTimeOffset||
|lastQuickScanSignatureVersion|String||
|lastReportedDateTime|DateTimeOffset||
|malwareProtectionEnabled|Boolean||
|networkInspectionSystemEnabled|Boolean||
|quickScanOverdue|Boolean||
|realTimeProtectionEnabled|Boolean||
|rebootRequired|Boolean||
|signatureUpdateOverdue|Boolean||
|signatureVersion|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|detectedMalwareState|[windowsDeviceMalwareState](../resources/windowsdevicemalwarestate.md) collection||

## JSON representation
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

