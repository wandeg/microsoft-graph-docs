---
title: "permissionScope resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# permissionScope resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|adminConsentDescription|String||
|adminConsentDisplayName|String||
|id|Guid||
|isEnabled|Boolean||
|origin|String||
|type|String||
|userConsentDescription|String||
|userConsentDisplayName|String||
|value|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.permissionScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.permissionScope",
  "adminConsentDescription": "String",
  "adminConsentDisplayName": "String",
  "id": "String (identifier)",
  "isEnabled": true,
  "origin": "String",
  "type": "String",
  "userConsentDescription": "String",
  "userConsentDisplayName": "String",
  "value": "String"
}
```

