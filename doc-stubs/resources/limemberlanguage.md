---
title: "LIMemberLanguage resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# LIMemberLanguage resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|name|[MultiLocaleString](../resources/multilocalestring.md)|**TODO: Add Description**|
|proficiency|LIMemberLanguageProficiency|**TODO: Add Description**. Possible values are: `ELEMENTARY`, `LIMITED_WORKING`, `PROFESSIONAL_WORKING`, `FULL_PROFESSIONAL`, `NATIVE_OR_BILINGUAL`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIMemberLanguage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIMemberLanguage",
  "name": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "proficiency": "String"
}
```

