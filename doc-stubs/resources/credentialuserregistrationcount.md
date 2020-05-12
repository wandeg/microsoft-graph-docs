---
title: "credentialUserRegistrationCount resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# credentialUserRegistrationCount resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|totalUserCount|Int64|**TODO: Add Description**|
|userRegistrationCounts|[userRegistrationCount](../resources/userregistrationcount.md) collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.credentialUserRegistrationCount",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.credentialUserRegistrationCount",
  "id": "String (identifier)",
  "totalUserCount": "Integer",
  "userRegistrationCounts": [
    {
      "@odata.type": "microsoft.graph.userRegistrationCount"
    }
  ]
}
```

