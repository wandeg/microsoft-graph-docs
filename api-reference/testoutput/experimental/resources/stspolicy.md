---
title: "stsPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# stsPolicy resource type


Namespace: microsoft.graph




Inherits from [policyBase](../resources/policybase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List stsPolicies](../api/stspolicy-list.md)|[stsPolicy](../resources/stspolicy.md) collection|List properties and relationships of the [stsPolicy](../resources/stspolicy.md) objects.|
|[Get stsPolicy](../api/stspolicy-get.md)|[stsPolicy](../resources/stspolicy.md)|Read properties and relationships of the [stsPolicy](../resources/stspolicy.md) object.|
|[List appliesTo](../api/stspolicy-list-appliesto.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the appliesTo navigation property.|
|[Create appliesTo](../api/stspolicy-post-appliesto.md)|[directoryObject](../resources/directoryobject.md)|Create appliesTo by posting to the appliesTo collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|definition|String collection||
|description|String| Inherited from [policyBase](../resources/policybase.md)|
|displayName|String| Inherited from [policyBase](../resources/policybase.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|isOrganizationDefault|Boolean||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliesTo|[directoryObject](../resources/directoryobject.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.stsPolicy",
  "baseType": "microsoft.graph.policyBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.stsPolicy",
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "definition": [
    "String"
  ],
  "isOrganizationDefault": true
}
```

