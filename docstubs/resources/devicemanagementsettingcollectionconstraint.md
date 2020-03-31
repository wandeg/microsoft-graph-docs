---
title: "deviceManagementSettingCollectionConstraint resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementSettingCollectionConstraint resource type


Namespace: microsoft.graph




Inherits from [deviceManagementConstraint](../resources/devicemanagementconstraint.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|maximumLength|Int32||
|minimumLength|Int32||

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

