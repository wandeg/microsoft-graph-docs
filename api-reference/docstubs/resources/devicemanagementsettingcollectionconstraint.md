---
title: "deviceManagementSettingCollectionConstraint resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementSettingCollectionConstraint resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [deviceManagementConstraint](../resources/devicemanagementconstraint.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|maximumLength|Int32|The maximum number of elements in the collection|
|minimumLength|Int32|The minimum number of elements in the collection|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingCollectionConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCollectionConstraint",
  "minimumLength": 1024,
  "maximumLength": 1024
}
```

