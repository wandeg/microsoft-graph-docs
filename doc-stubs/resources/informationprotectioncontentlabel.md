---
title: "informationProtectionContentLabel resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# informationProtectionContentLabel resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignmentMethod|assignmentMethod|**TODO: Add Description**. Possible values are: `standard`, `privileged`, `auto`.|
|creationDateTime|DateTimeOffset|**TODO: Add Description**|
|label|[labelDetails](../resources/labeldetails.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.informationProtectionContentLabel"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.informationProtectionContentLabel",
  "creationDateTime": "String (timestamp)",
  "assignmentMethod": "String",
  "label": {
    "@odata.type": "microsoft.graph.labelDetails"
  }
}
```

