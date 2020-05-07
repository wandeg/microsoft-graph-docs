---
title: "deviceConfigurationUserStateSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceConfigurationUserStateSummary resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|compliantUserCount|Int32|**TODO: Add Description**|
|conflictUserCount|Int32|**TODO: Add Description**|
|errorUserCount|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|nonCompliantUserCount|Int32|**TODO: Add Description**|
|notApplicableUserCount|Int32|**TODO: Add Description**|
|remediatedUserCount|Int32|**TODO: Add Description**|
|unknownUserCount|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationUserStateSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "id": "String (identifier)",
  "unknownUserCount": "Integer",
  "notApplicableUserCount": "Integer",
  "compliantUserCount": "Integer",
  "remediatedUserCount": "Integer",
  "nonCompliantUserCount": "Integer",
  "errorUserCount": "Integer",
  "conflictUserCount": "Integer"
}
```

