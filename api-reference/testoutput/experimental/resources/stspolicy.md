---
title: "stsPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# stsPolicy resource type




Inherits from [policyBase](../resources/policyBase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List stsPolicies](../api/stspolicy-list.md)|[stsPolicy](../resources/stsPolicy.md) collection|List properties and relationships of the [stsPolicy](../resources/stspolicy.md) objects.|
|[Get stsPolicy](../api/stspolicy-get.md)|[stsPolicy](../resources/stsPolicy.md)|Read properties and relationships of the [stsPolicy](../resources/stspolicy.md) object.|
|[List appliesTo](../api/stspolicy-list-appliesto.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the appliesTo navigation property.|
|[Create appliesTo](../api/stspolicy-post-appliesto.md)|[directoryObject](../resources/directoryObject.md)|Create appliesTo by posting to the appliesTo collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|definition|String collection||
|description|String| Inherited from [policyBase](../resources/policyBase.md)|
|displayName|String| Inherited from [policyBase](../resources/policyBase.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|isOrganizationDefault|Boolean||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliesTo|[directoryObject](../resources/directoryObject.md) collection||

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

