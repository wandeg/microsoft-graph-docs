---
title: "governanceRoleAssignmentRequestStatus resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# governanceRoleAssignmentRequestStatus resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|status|String||
|statusDetails|[keyValue](../resources/keyValue.md) collection||
|subStatus|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.governanceRoleAssignmentRequestStatus",
  "status": "String",
  "subStatus": "String",
  "statusDetails": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "String",
      "value": "String"
    }
  ]
}
```

