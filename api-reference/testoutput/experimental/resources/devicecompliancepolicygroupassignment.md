---
title: "deviceCompliancePolicyGroupAssignment resource type"
description: "Device compliance policy group assignment."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceCompliancePolicyGroupAssignment resource type

Device compliance policy group assignment.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceCompliancePolicyGroupAssignments](../api/devicecompliancepolicygroupassignment-list.md)|[deviceCompliancePolicyGroupAssignment](../resources/deviceCompliancePolicyGroupAssignment.md) collection|List properties and relationships of the [deviceCompliancePolicyGroupAssignment](../resources/devicecompliancepolicygroupassignment.md) objects.|
|[Get deviceCompliancePolicyGroupAssignment](../api/devicecompliancepolicygroupassignment-get.md)|[deviceCompliancePolicyGroupAssignment](../resources/deviceCompliancePolicyGroupAssignment.md)|Read properties and relationships of the [deviceCompliancePolicyGroupAssignment](../resources/devicecompliancepolicygroupassignment.md) object.|
|[Create deviceCompliancePolicyGroupAssignment](../api/devicecompliancepolicygroupassignment-create.md)|[deviceCompliancePolicyGroupAssignment](../resources/deviceCompliancePolicyGroupAssignment.md)|Create a new [deviceCompliancePolicyGroupAssignment](../resources/devicecompliancepolicygroupassignment.md) object.|
|[Delete deviceCompliancePolicyGroupAssignment](../api/devicecompliancepolicygroupassignment-delete.md)|None|Deletes a [deviceCompliancePolicyGroupAssignment](../resources/devicecompliancepolicygroupassignment.md).|
|[Update deviceCompliancePolicyGroupAssignment](../api/devicecompliancepolicygroupassignment-update.md)|[deviceCompliancePolicyGroupAssignment](../resources/deviceCompliancePolicyGroupAssignment.md)|Update the properties of a [deviceCompliancePolicyGroupAssignment](../resources/devicecompliancepolicygroupassignment.md) object.|
|[Get deviceCompliancePolicy](../api/devicecompliancepolicy-get.md)|[deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|Read properties and relationships of the [deviceCompliancePolicy](../resources/devicecompliancepolicy.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|excludeGroup|Boolean|Indicates if this group is should be excluded. Defaults that the group should be included|
|id|String| Inherited from [entity](../resources/entity.md)|
|targetGroupId|String|The Id of the AAD group we are targeting the device compliance policy to.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deviceCompliancePolicy|[deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|The navigation link to the  device compliance polic targeted.|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyGroupAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String",
  "excludeGroup": true
}
```

