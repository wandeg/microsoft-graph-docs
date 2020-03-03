---
title: "mobileAppAssignment resource type"
description: "A class containing the properties used for Group Assignment of a Mobile App."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mobileAppAssignment resource type


Namespace: microsoft.graph

A class containing the properties used for Group Assignment of a Mobile App.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List mobileAppAssignments](../api/mobileappassignment-list.md)|[mobileAppAssignment](../resources/mobileappassignment.md) collection|List properties and relationships of the [mobileAppAssignment](../resources/mobileappassignment.md) objects.|
|[Get mobileAppAssignment](../api/mobileappassignment-get.md)|[mobileAppAssignment](../resources/mobileappassignment.md)|Read properties and relationships of the [mobileAppAssignment](../resources/mobileappassignment.md) object.|
|[Create mobileAppAssignment](../api/mobileappassignment-create.md)|[mobileAppAssignment](../resources/mobileappassignment.md)|Create a new [mobileAppAssignment](../resources/mobileappassignment.md) object.|
|[Delete mobileAppAssignment](../api/mobileappassignment-delete.md)|None|Deletes a [mobileAppAssignment](../resources/mobileappassignment.md).|
|[Update mobileAppAssignment](../api/mobileappassignment-update.md)|[mobileAppAssignment](../resources/mobileappassignment.md)|Update the properties of a [mobileAppAssignment](../resources/mobileappassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|intent|Enumeration|The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|
|settings|[mobileAppAssignmentSettings](../resources/mobileappassignmentsettings.md)|The settings for target assignment defined by the admin.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)|The target group assignment defined by the admin.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "String (identifier)",
  "intent": "String",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

