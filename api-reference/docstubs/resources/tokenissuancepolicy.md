---
title: "tokenIssuancePolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# tokenIssuancePolicy resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [stsPolicy](../resources/stspolicy.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get tokenIssuancePolicy](../api/tokenissuancepolicy-get.md)|[tokenIssuancePolicy](../resources/tokenissuancepolicy.md)|Read the properties and relationships of a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.|
|[Update tokenIssuancePolicy](../api/tokenissuancepolicy-update.md)|[tokenIssuancePolicy](../resources/tokenissuancepolicy.md)|Update the properties of a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.|
|[List appliesTo](../api/tokenissuancepolicy-list-appliesto.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the appliesTo navigation property.|
|[Add appliesTo](../api/tokenissuancepolicy-post-appliesto.md)|[directoryObject](../resources/directoryobject.md)|Add appliesTo by posting to the appliesTo collection.|
|[Remove appliesTo](../api/tokenissuancepolicy-delete-appliesto.md)|None|Remove an [directoryObject](../resources/directoryobject.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|definition|String collection|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md)|
|description|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|displayName|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isOrganizationDefault|Boolean|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliesTo|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md)|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.tokenIssuancePolicy",
  "baseType": "microsoft.graph.stsPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.tokenIssuancePolicy",
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "definition": [
    "String"
  ],
  "isOrganizationDefault": true
}
```

