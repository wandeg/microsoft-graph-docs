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
|[List scheduledActionsForRule](../api/intune-devicecompliancepolicy-list-scheduledactionsforrule.md)|[deviceComplianceScheduledActionForRule](../resources/intune-devicecompliancescheduledactionforrule.md) collection|Get the deviceComplianceScheduledActionForRules from the scheduledActionsForRule navigation property.|
|[Create scheduledActionsForRule](../api/intune-devicecompliancepolicy-post-scheduledactionsforrule.md)|[deviceComplianceScheduledActionForRule](../resources/intune-devicecompliancescheduledactionforrule.md)|Create a new scheduledActionsForRule object.|
|[Delete scheduledActionsForRule](../api/intune-devicecompliancepolicy-delete-scheduledactionsforrule.md)|None|Delete a [deviceComplianceScheduledActionForRule](../resources/intune-devicecompliancescheduledactionforrule.md) object.|
|[Update scheduledActionsForRule](../api/intune-devicecompliancepolicy-update-scheduledactionsforrule.md)|[deviceComplianceScheduledActionForRule](../resources/intune-devicecompliancescheduledactionforrule.md)|Update the properties of a scheduledActionsForRule object.|
|[Get scheduledActionsForRule](../api/intune-devicecompliancepolicy-get-devicecompliancescheduledactionforrule.md)|[deviceComplianceScheduledActionForRule](../resources/intune-devicecompliancescheduledactionforrule.md)|Read the properties and relationships of a [deviceComplianceScheduledActionForRule](../resources/intune-devicecompliancescheduledactionforrule.md) object.|
|[List scheduledActionConfigurations](../api/intune-devicecompliancescheduledactionforrule-list-scheduledactionconfigurations.md)|[deviceComplianceActionItem](../resources/intune-devicecomplianceactionitem.md) collection|Get the deviceComplianceActionItems from the scheduledActionConfigurations navigation property.|
|[Create scheduledActionConfigurations](../api/intune-devicecompliancescheduledactionforrule-post-scheduledactionconfigurations.md)|[deviceComplianceActionItem](../resources/intune-devicecomplianceactionitem.md)|Create a new scheduledActionConfigurations object.|
|[Delete scheduledActionConfigurations](../api/intune-devicecompliancescheduledactionforrule-delete-scheduledactionconfigurations.md)|None|Delete a [deviceComplianceActionItem](../resources/intune-devicecomplianceactionitem.md) object.|
|[Update scheduledActionConfigurations](../api/intune-devicecompliancescheduledactionforrule-update-scheduledactionconfigurations.md)|[deviceComplianceActionItem](../resources/intune-devicecomplianceactionitem.md)|Update the properties of a scheduledActionConfigurations object.|
|[Get scheduledActionConfigurations](../api/intune-devicecompliancescheduledactionforrule-get-devicecomplianceactionitem.md)|[deviceComplianceActionItem](../resources/intune-devicecomplianceactionitem.md)|Read the properties and relationships of a [deviceComplianceActionItem](../resources/intune-devicecomplianceactionitem.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|ruleName|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|scheduledActionConfigurations|[deviceComplianceActionItem](../resources/intune-devicecomplianceactionitem.md) collection|**TODO: Add Description**|

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

