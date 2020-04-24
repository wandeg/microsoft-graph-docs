---
title: "windowsProtectionState resource type"
description: "Device protection status entity."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsProtectionState resource type


Namespace: microsoft.graph

Device protection status entity.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsProtectionState](../api/windowsprotectionstate-get.md)|[windowsProtectionState](../resources/windowsprotectionstate.md)|Read the properties and relationships of a [windowsProtectionState](../resources/windowsprotectionstate.md) object.|
|[Update windowsProtectionState](../api/windowsprotectionstate-update.md)|[windowsProtectionState](../resources/windowsprotectionstate.md)|Update the properties of a [windowsProtectionState](../resources/windowsprotectionstate.md) object.|
|[List detectedMalwareState](../api/windowsprotectionstate-list-detectedmalwarestate.md)|[windowsDeviceMalwareState](../resources/windowsdevicemalwarestate.md) collection|Get the windowsDeviceMalwareStates from the detectedMalwareState navigation property.|
|[Create detectedMalwareState](../api/windowsprotectionstate-post-detectedmalwarestate.md)|[windowsDeviceMalwareState](../resources/windowsdevicemalwarestate.md)|Create a new detectedMalwareState object.|
|[Delete detectedMalwareState](../api/windowsprotectionstate-delete-detectedmalwarestate.md)|None|Delete a [windowsDeviceMalwareState](../resources/windowsdevicemalwarestate.md) object.|
|[Update detectedMalwareState](../api/windowsprotectionstate-update-detectedmalwarestate.md)|[windowsDeviceMalwareState](../resources/windowsdevicemalwarestate.md)|Update the properties of a detectedMalwareState object.|
|[Get windowsDeviceMalwareState](../api/windowsdevicemalwarestate-get.md)|[windowsDeviceMalwareState](../resources/windowsdevicemalwarestate.md)|Read the properties and relationships of a [windowsDeviceMalwareState](../resources/windowsdevicemalwarestate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|antiMalwareVersion|String|Current anti malware version|
|deviceState|windowsDeviceHealthState|Computer's state (like clean or pending full scan or pending reboot etc). Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|engineVersion|String|Current endpoint protection engine's version|
|fullScanOverdue|Boolean|Full scan overdue or not?|
|fullScanRequired|Boolean|Full scan required or not?|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
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
|detectedMalwareState|[windowsDeviceMalwareState](../resources/windowsdevicemalwarestate.md) collection|Device malware list|

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

