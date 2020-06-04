---
title: "claimsMappingPolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# claimsMappingPolicy resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [stsPolicy](../resources/stspolicy.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List claimsMappingPolicies](../api/claimsmappingpolicy-list.md)|[claimsMappingPolicy](../resources/claimsmappingpolicy.md) collection|Get a list of the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects and their properties.|
|[Create claimsMappingPolicy](../api/claimsmappingpolicy-create.md)|[claimsMappingPolicy](../resources/claimsmappingpolicy.md)|Create a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.|
|[Get claimsMappingPolicy](../api/claimsmappingpolicy-get.md)|[claimsMappingPolicy](../resources/claimsmappingpolicy.md)|Read the properties and relationships of a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.|
|[Update claimsMappingPolicy](../api/claimsmappingpolicy-update.md)|[claimsMappingPolicy](../resources/claimsmappingpolicy.md)|Update the properties of a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.|
|[Delete claimsMappingPolicy](../api/claimsmappingpolicy-delete.md)|None|Deletes a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.|
|[List appliesTo](../api/claimsmappingpolicy-list-appliesto.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the appliesTo navigation property.|
|[Add appliesTo](../api/claimsmappingpolicy-post-appliesto.md)|[directoryObject](../resources/directoryobject.md)|Add appliesTo by posting to the appliesTo collection.|
|[Remove appliesTo](../api/claimsmappingpolicy-delete-appliesto.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|definition|String collection|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|displayName|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isOrganizationDefault|Boolean|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliesTo|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md)|

## JSON representation
The following is a JSON representation of the resource.
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
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "definition": [
    "String"
  ],
  "isOrganizationDefault": "Boolean"
}
```

