---
title: "deviceAppManagementTask resource type"
description: "A device app management task."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceAppManagementTask resource type


Namespace: microsoft.graph

A device app management task.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceAppManagementTask](../api/deviceappmanagementtask-get.md)|[deviceAppManagementTask](../resources/deviceappmanagementtask.md)|Read properties and relationships of the [deviceAppManagementTask](../resources/deviceappmanagementtask.md) object.|
|[Update deviceAppManagementTask](../api/deviceappmanagementtask-update.md)|[deviceAppManagementTask](../resources/deviceappmanagementtask.md)|Update the properties of a [deviceAppManagementTask](../resources/deviceappmanagementtask.md) object.|
|[updateStatus](../api/deviceappmanagementtask-updatestatus.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedTo|String|The name or email of the admin this task is assigned to.|
|category|Enumeration|The category. Possible values are: `unknown`, `advancedThreatProtection`.|
|createdDateTime|DateTimeOffset|The created date.|
|creator|String|The email address of the creator.|
|creatorNotes|String|Notes from the creator.|
|description|String|The description.|
|displayName|String|The name.|
|dueDateTime|DateTimeOffset|The due date.|
|id|String| Inherited from [entity](../resources/entity.md)|
|priority|Enumeration|The priority. Possible values are: `none`, `high`, `low`.|
|status|Enumeration|The status. Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagementTask",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "category": "String",
  "priority": "String",
  "creator": "String",
  "creatorNotes": "String",
  "assignedTo": "String",
  "status": "String"
}
```

