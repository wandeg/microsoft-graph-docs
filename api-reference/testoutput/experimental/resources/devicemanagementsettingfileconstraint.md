---
title: "deviceManagementSettingFileConstraint resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementSettingFileConstraint resource type


Namespace: microsoft.graph




Inherits from [deviceManagementConstraint](../resources/devicemanagementconstraint.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|supportedExtensions|String collection|Acceptable file extensions to upload for this setting|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingFileConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingFileConstraint",
  "supportedExtensions": [
    "String"
  ]
}
```

