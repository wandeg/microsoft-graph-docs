---
title: "managedEBookAssignment resource type"
description: "Contains properties used to assign a eBook to a group."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# managedEBookAssignment resource type

Contains properties used to assign a eBook to a group.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedEBookAssignment](../api/managedebookassignment-get.md)|[managedEBookAssignment](../resources/managedEBookAssignment.md)|Read properties and relationships of the [managedEBookAssignment](../resources/managedebookassignment.md) object.|
|[Delete managedEBookAssignment](../api/managedebookassignment-delete.md)|None|Deletes a [managedEBookAssignment](../resources/managedebookassignment.md).|
|[Update managedEBookAssignment](../api/managedebookassignment-update.md)|[managedEBookAssignment](../resources/managedEBookAssignment.md)|Update the properties of a [managedEBookAssignment](../resources/managedebookassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|installIntent|Enumeration|The install intent for eBook. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceAndAppManagementAssignmentTarget.md)|The assignment target for eBook.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```

