---
title: "dlpPoliciesJobResult resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# dlpPoliciesJobResult resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|matchingRules|[matchingDlpRule](../resources/matchingdlprule.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.dlpPoliciesJobResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dlpPoliciesJobResult",
  "matchingRules": [
    {
      "@odata.type": "microsoft.graph.matchingDlpRule",
      "ruleId": "String",
      "ruleName": "String",
      "policyId": "String",
      "policyName": "String",
      "isMostRestrictive": true,
      "priority": 1024,
      "actions": [
        {
          "@odata.type": "microsoft.graph.dlpActionInfo",
          "action": "String"
        }
      ],
      "ruleMode": "String"
    }
  ]
}
```

