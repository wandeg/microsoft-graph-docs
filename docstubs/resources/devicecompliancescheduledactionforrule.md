---
title: "deviceComplianceScheduledActionForRule resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceComplianceScheduledActionForRule resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceComplianceScheduledActionForRule](../api/devicecompliancescheduledactionforrule-get.md)|[deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md)|Read properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md) object.|
|[Update deviceComplianceScheduledActionForRule](../api/devicecompliancescheduledactionforrule-update.md)|[deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md)|Update the properties of a [deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md) object.|
|[List scheduledActionConfigurations](../api/devicecompliancescheduledactionforrule-list-scheduledactionconfigurations.md)|[deviceComplianceActionItem](../resources/devicecomplianceactionitem.md) collection|Get the deviceComplianceActionItems from the scheduledActionConfigurations navigation property.|
|[Add scheduledActionConfigurations](../api/devicecompliancescheduledactionforrule-post-scheduledactionconfigurations.md)|[deviceComplianceActionItem](../resources/devicecomplianceactionitem.md)|Add scheduledActionConfigurations by posting to the scheduledActionConfigurations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|ruleName|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|scheduledActionConfigurations|[deviceComplianceActionItem](../resources/devicecomplianceactionitem.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScheduledActionForRule",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "String (identifier)",
  "ruleName": "String"
}
```

