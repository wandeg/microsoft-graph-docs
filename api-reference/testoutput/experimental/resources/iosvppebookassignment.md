---
title: "iosVppEBookAssignment resource type"
description: "Contains properties used to assign an iOS VPP EBook to a group."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosVppEBookAssignment resource type


Namespace: microsoft.graph

Contains properties used to assign an iOS VPP EBook to a group.


Inherits from [managedEBookAssignment](../resources/managedebookassignment.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List iosVppEBookAssignments](../api/iosvppebookassignment-list.md)|[iosVppEBookAssignment](../resources/iosvppebookassignment.md) collection|List properties and relationships of the [iosVppEBookAssignment](../resources/iosvppebookassignment.md) objects.|
|[Get iosVppEBookAssignment](../api/iosvppebookassignment-get.md)|[iosVppEBookAssignment](../resources/iosvppebookassignment.md)|Read properties and relationships of the [iosVppEBookAssignment](../resources/iosvppebookassignment.md) object.|
|[Create iosVppEBookAssignment](../api/iosvppebookassignment-create.md)|[iosVppEBookAssignment](../resources/iosvppebookassignment.md)|Create a new [iosVppEBookAssignment](../resources/iosvppebookassignment.md) object.|
|[Delete iosVppEBookAssignment](../api/iosvppebookassignment-delete.md)|None|Deletes a [iosVppEBookAssignment](../resources/iosvppebookassignment.md).|
|[Update iosVppEBookAssignment](../api/iosvppebookassignment-update.md)|[iosVppEBookAssignment](../resources/iosvppebookassignment.md)|Update the properties of a [iosVppEBookAssignment](../resources/iosvppebookassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|installIntent|Enumeration|The install intent for eBook. Inherited from [managedEBookAssignment](../resources/managedebookassignment.md). Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-apps-deviceandappmanagementassignmenttarget.md)|The assignment target for eBook. Inherited from [managedEBookAssignment](../resources/managedebookassignment.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBookAssignment",
  "baseType": "microsoft.graph.managedEBookAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```

