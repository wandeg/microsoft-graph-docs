---
title: "deviceCompliancePolicyDeviceStateSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceCompliancePolicyDeviceStateSummary resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|compliantDeviceCount|Int32|**TODO: Add Description**|
|configManagerCount|Int32|**TODO: Add Description**|
|conflictDeviceCount|Int32|**TODO: Add Description**|
|errorDeviceCount|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|inGracePeriodCount|Int32|**TODO: Add Description**|
|nonCompliantDeviceCount|Int32|**TODO: Add Description**|
|notApplicableDeviceCount|Int32|**TODO: Add Description**|
|remediatedDeviceCount|Int32|**TODO: Add Description**|
|unknownDeviceCount|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "id": "String (identifier)",
  "inGracePeriodCount": "Integer",
  "configManagerCount": "Integer",
  "unknownDeviceCount": "Integer",
  "notApplicableDeviceCount": "Integer",
  "compliantDeviceCount": "Integer",
  "remediatedDeviceCount": "Integer",
  "nonCompliantDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "conflictDeviceCount": "Integer"
}
```

