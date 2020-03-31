---
title: "LISkillArray resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# LISkillArray resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|skills|[LISkill](../resources/liskill.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LISkillArray"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LISkillArray",
  "skills": [
    {
      "@odata.type": "microsoft.graph.LISkill",
      "id": "String",
      "name": {
        "@odata.type": "microsoft.graph.MultiLocaleString",
        "localized": [
          {
            "@odata.type": "microsoft.graph.StringMapElement",
            "key": "String",
            "value": "String"
          }
        ],
        "preferredLocale": {
          "@odata.type": "microsoft.graph.Locale",
          "language": "String",
          "country": "String",
          "variant": "String"
        }
      }
    }
  ]
}
```

