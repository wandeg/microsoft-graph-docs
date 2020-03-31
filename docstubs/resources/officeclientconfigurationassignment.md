---
title: "officeClientConfigurationAssignment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# officeClientConfigurationAssignment resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get officeClientConfigurationAssignment](../api/officeclientconfigurationassignment-get.md)|[officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md)|Read properties and relationships of the [officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md) object.|
|[Update officeClientConfigurationAssignment](../api/officeclientconfigurationassignment-update.md)|[officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md)|Update the properties of a [officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|target|[officeConfigurationAssignmentTarget](../resources/officeconfigurationassignmenttarget.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientConfigurationAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

