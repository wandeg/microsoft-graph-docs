---
title: "deviceComplianceScheduledActionForRule resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceComplianceScheduledActionForRule resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List scheduledActionConfigurations](../api/devicecompliancescheduledactionforrule-list-scheduledactionconfigurations.md)|[deviceComplianceActionItem](../resources/devicecomplianceactionitem.md) collection|Get the deviceComplianceActionItems from the scheduledActionConfigurations navigation property.|
|[Create scheduledActionConfigurations](../api/devicecompliancescheduledactionforrule-post-scheduledactionconfigurations.md)|[deviceComplianceActionItem](../resources/devicecomplianceactionitem.md)|Create a new scheduledActionConfigurations object.|
|[Delete scheduledActionConfigurations](../api/devicecompliancescheduledactionforrule-delete-scheduledactionconfigurations.md)|None|Delete a [deviceComplianceActionItem](../resources/devicecomplianceactionitem.md) object.|
|[Update scheduledActionConfigurations](../api/devicecompliancescheduledactionforrule-update-scheduledactionconfigurations.md)|[deviceComplianceActionItem](../resources/devicecomplianceactionitem.md)|Update the properties of a scheduledActionConfigurations object.|
|[Get deviceComplianceActionItem](../api/devicecomplianceactionitem-get.md)|[deviceComplianceActionItem](../resources/devicecomplianceactionitem.md)|Read the properties and relationships of a [deviceComplianceActionItem](../resources/devicecomplianceactionitem.md) object.|
|[List scheduledActionsForRule](../api/devicecompliancepolicy-list-scheduledactionsforrule.md)|[deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md) collection|Get the deviceComplianceScheduledActionForRules from the scheduledActionsForRule navigation property.|
|[Create scheduledActionsForRule](../api/devicecompliancepolicy-post-scheduledactionsforrule.md)|[deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md)|Create a new scheduledActionsForRule object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|ruleName|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|scheduledActionConfigurations|[deviceComplianceActionItem](../resources/devicecomplianceactionitem.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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

