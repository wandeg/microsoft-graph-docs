---
title: "windowsProtectionState resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsProtectionState resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List detectedMalwareState](../api/windowsprotectionstate-list-detectedmalwarestate.md)|[windowsDeviceMalwareState](../resources/windowsdevicemalwarestate.md) collection|Get the windowsDeviceMalwareStates from the detectedMalwareState navigation property.|
|[Create detectedMalwareState](../api/windowsprotectionstate-post-detectedmalwarestate.md)|[windowsDeviceMalwareState](../resources/windowsdevicemalwarestate.md)|Create a new detectedMalwareState object.|
|[Delete detectedMalwareState](../api/windowsprotectionstate-delete-detectedmalwarestate.md)|None|Delete a [windowsDeviceMalwareState](../resources/windowsdevicemalwarestate.md) object.|
|[Update detectedMalwareState](../api/windowsprotectionstate-update-detectedmalwarestate.md)|[windowsDeviceMalwareState](../resources/windowsdevicemalwarestate.md)|Update the properties of a detectedMalwareState object.|
|[Get windowsDeviceMalwareState](../api/windowsdevicemalwarestate-get.md)|[windowsDeviceMalwareState](../resources/windowsdevicemalwarestate.md)|Read the properties and relationships of a [windowsDeviceMalwareState](../resources/windowsdevicemalwarestate.md) object.|
|[List windowsProtectionState](../api/manageddevice-list-windowsprotectionstate.md)|[windowsProtectionState](../resources/windowsprotectionstate.md) collection|Get the windowsProtectionStates from the windowsProtectionState navigation property.|
|[Create windowsProtectionState](../api/manageddevice-post-windowsprotectionstate.md)|[windowsProtectionState](../resources/windowsprotectionstate.md)|Create a new windowsProtectionState object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|antiMalwareVersion|String|**TODO: Add Description**|
|deviceState|windowsDeviceHealthState|**TODO: Add Description**. Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|engineVersion|String|**TODO: Add Description**|
|fullScanOverdue|Boolean|**TODO: Add Description**|
|fullScanRequired|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastFullScanDateTime|DateTimeOffset|**TODO: Add Description**|
|lastFullScanSignatureVersion|String|**TODO: Add Description**|
|lastQuickScanDateTime|DateTimeOffset|**TODO: Add Description**|
|lastQuickScanSignatureVersion|String|**TODO: Add Description**|
|lastReportedDateTime|DateTimeOffset|**TODO: Add Description**|
|malwareProtectionEnabled|Boolean|**TODO: Add Description**|
|networkInspectionSystemEnabled|Boolean|**TODO: Add Description**|
|quickScanOverdue|Boolean|**TODO: Add Description**|
|realTimeProtectionEnabled|Boolean|**TODO: Add Description**|
|rebootRequired|Boolean|**TODO: Add Description**|
|signatureUpdateOverdue|Boolean|**TODO: Add Description**|
|signatureVersion|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|detectedMalwareState|[windowsDeviceMalwareState](../resources/windowsdevicemalwarestate.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "malwareProtectionEnabled": "Boolean",
  "deviceState": "String",
  "realTimeProtectionEnabled": "Boolean",
  "networkInspectionSystemEnabled": "Boolean",
  "quickScanOverdue": "Boolean",
  "fullScanOverdue": "Boolean",
  "signatureUpdateOverdue": "Boolean",
  "rebootRequired": "Boolean",
  "fullScanRequired": "Boolean",
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

