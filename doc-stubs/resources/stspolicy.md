---
title: "stsPolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# stsPolicy resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [policyBase](../resources/policybase.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List stsPolicies](../api/stspolicy-list.md)|[stsPolicy](../resources/stspolicy.md) collection|Get a list of the [stsPolicy](../resources/stspolicy.md) objects and their properties.|
|[Create stsPolicy](../api/stspolicy-create.md)|[stsPolicy](../resources/stspolicy.md)|Create a new [stsPolicy](../resources/stspolicy.md) object.|
|[Get stsPolicy](../api/stspolicy-get.md)|[stsPolicy](../resources/stspolicy.md)|Read the properties and relationships of a [stsPolicy](../resources/stspolicy.md) object.|
|[Update stsPolicy](../api/stspolicy-update.md)|[stsPolicy](../resources/stspolicy.md)|Update the properties of a [stsPolicy](../resources/stspolicy.md) object.|
|[Delete stsPolicy](../api/stspolicy-delete.md)|None|Deletes a [stsPolicy](../resources/stspolicy.md) object.|
|[List appliesTo](../api/stspolicy-list-appliesto.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the appliesTo navigation property.|
|[Add appliesTo](../api/stspolicy-post-appliesto.md)|[directoryObject](../resources/directoryobject.md)|Add appliesTo by posting to the appliesTo collection.|
|[Remove appliesTo](../api/stspolicy-delete-appliesto.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|definition|String collection|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|displayName|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isOrganizationDefault|Boolean|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliesTo|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "definition": [
    "String"
  ],
  "isOrganizationDefault": "Boolean"
}
```

