---
title: "mobileAppAssignment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mobileAppAssignment resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get mobileAppAssignment](../api/mobileappassignment-get.md)|[mobileAppAssignment](../resources/mobileappassignment.md)|Read properties and relationships of the [mobileAppAssignment](../resources/mobileappassignment.md) object.|
|[Update mobileAppAssignment](../api/mobileappassignment-update.md)|[mobileAppAssignment](../resources/mobileappassignment.md)|Update the properties of a [mobileAppAssignment](../resources/mobileappassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|intent|Enumeration| Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|
|settings|[mobileAppAssignmentSettings](../resources/mobileappassignmentsettings.md)||
|source|Enumeration| Possible values are: `direct`, `policySets`.|
|sourceId|String||
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)||

## Relationships
None

## JSON representation
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
  },
  "source": "String",
  "sourceId": "String"
}
```

