---
title: "educationSynchronizationLicenseAssignment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationSynchronizationLicenseAssignment resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|appliesTo|Enumeration|. Possible values are: `student`, `teacher`, `none`, `unknownFutureValue`, `faculty`.|
|skuIds|String collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationSynchronizationLicenseAssignment",
  "appliesTo": "String",
  "skuIds": [
    "String"
  ]
}
```

