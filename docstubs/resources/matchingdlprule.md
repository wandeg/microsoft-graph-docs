---
title: "matchingDlpRule resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# matchingDlpRule resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|actions|[dlpActionInfo](../resources/dlpactioninfo.md) collection||
|isMostRestrictive|Boolean||
|policyId|String||
|policyName|String||
|priority|Int32||
|ruleId|String||
|ruleMode|Enumeration| Possible values are: `audit`, `auditAndNotify`, `enforce`, `pendingDeletion`, `test`.|
|ruleName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.matchingDlpRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.matchingDlpRule",
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
```

