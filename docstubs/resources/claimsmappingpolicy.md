---
title: "claimsMappingPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# claimsMappingPolicy resource type


Namespace: microsoft.graph




Inherits from [stsPolicy](../resources/stspolicy.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get claimsMappingPolicy](../api/claimsmappingpolicy-get.md)|[claimsMappingPolicy](../resources/claimsmappingpolicy.md)|Read properties and relationships of the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.|
|[Update claimsMappingPolicy](../api/claimsmappingpolicy-update.md)|[claimsMappingPolicy](../resources/claimsmappingpolicy.md)|Update the properties of a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.|
|[List appliesTo](../api/claimsmappingpolicy-list-appliesto.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the appliesTo navigation property.|
|[Create appliesTo](../api/claimsmappingpolicy-post-appliesto.md)|[directoryObject](../resources/directoryobject.md)|Create appliesTo by posting to the appliesTo collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|definition|String collection| Inherited from [stsPolicy](../resources/stspolicy.md)|
|description|String| Inherited from [policyBase](../resources/policybase.md)|
|displayName|String| Inherited from [policyBase](../resources/policybase.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|isOrganizationDefault|Boolean| Inherited from [stsPolicy](../resources/stspolicy.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliesTo|[directoryObject](../resources/directoryobject.md) collection| Inherited from [stsPolicy](../resources/stspolicy.md)|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.claimsMappingPolicy",
  "baseType": "microsoft.graph.stsPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.claimsMappingPolicy",
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "definition": [
    "String"
  ],
  "isOrganizationDefault": true
}
```

