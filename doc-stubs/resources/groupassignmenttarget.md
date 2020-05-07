---
title: "groupAssignmentTarget resource type"
description: "Represents an assignment to a group."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# groupAssignmentTarget resource type


Namespace: microsoft.graph

Represents an assignment to a group.


Inherits from [deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|groupId|String|The group Id that is the target of the assignment.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.management.services.api.groupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.groupAssignmentTarget",
  "groupId": "String"
}
```

