---
title: "managedEBookAssignment resource type"
description: "Contains properties used to assign a eBook to a group."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedEBookAssignment resource type


Namespace: microsoft.graph

Contains properties used to assign a eBook to a group.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List managedEBookAssignments](../api/managedebookassignment-list.md)|[managedEBookAssignment](../resources/managedebookassignment.md) collection|List properties and relationships of the [managedEBookAssignment](../resources/managedebookassignment.md) objects.|
|[Get managedEBookAssignment](../api/managedebookassignment-get.md)|[managedEBookAssignment](../resources/managedebookassignment.md)|Read properties and relationships of the [managedEBookAssignment](../resources/managedebookassignment.md) object.|
|[Create managedEBookAssignment](../api/managedebookassignment-create.md)|[managedEBookAssignment](../resources/managedebookassignment.md)|Create a new [managedEBookAssignment](../resources/managedebookassignment.md) object.|
|[Delete managedEBookAssignment](../api/managedebookassignment-delete.md)|None|Deletes a [managedEBookAssignment](../resources/managedebookassignment.md).|
|[Update managedEBookAssignment](../api/managedebookassignment-update.md)|[managedEBookAssignment](../resources/managedebookassignment.md)|Update the properties of a [managedEBookAssignment](../resources/managedebookassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|installIntent|Enumeration|The install intent for eBook. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)|The assignment target for eBook.|

## Relationships
None

## JSON representation
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

