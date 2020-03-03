---
title: "claimsMappingPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# claimsMappingPolicy resource type




Inherits from [stsPolicy](../resources/stsPolicy.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get claimsMappingPolicy](../api/claimsmappingpolicy-get.md)|[claimsMappingPolicy](../resources/claimsMappingPolicy.md)|Read properties and relationships of the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.|
|[Delete claimsMappingPolicy](../api/claimsmappingpolicy-delete.md)|None|Deletes a [claimsMappingPolicy](../resources/claimsmappingpolicy.md).|
|[Update claimsMappingPolicy](../api/claimsmappingpolicy-update.md)|[claimsMappingPolicy](../resources/claimsMappingPolicy.md)|Update the properties of a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.|
|[List appliesTo](../api/claimsmappingpolicy-list-appliesto.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the appliesTo navigation property.|
|[Create appliesTo](../api/claimsmappingpolicy-post-appliesto.md)|[directoryObject](../resources/directoryObject.md)|Create appliesTo by posting to the appliesTo collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|definition|String collection| Inherited from [stsPolicy](../resources/stsPolicy.md)|
|description|String| Inherited from [policyBase](../resources/policyBase.md)|
|displayName|String| Inherited from [policyBase](../resources/policyBase.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|isOrganizationDefault|Boolean| Inherited from [stsPolicy](../resources/stsPolicy.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliesTo|[directoryObject](../resources/directoryObject.md) collection| Inherited from [stsPolicy](../resources/stsPolicy.md)|

## JSON Representation
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

