---
title: "passwordSingleSignOnCredentialSet resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# passwordSingleSignOnCredentialSet resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|credentials|[credential](../resources/credential.md) collection||
|id|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.passwordSingleSignOnCredentialSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordSingleSignOnCredentialSet",
  "id": "String (identifier)",
  "credentials": [
    {
      "@odata.type": "microsoft.graph.credential",
      "fieldId": "String",
      "value": "String",
      "type": "String"
    }
  ]
}
```

