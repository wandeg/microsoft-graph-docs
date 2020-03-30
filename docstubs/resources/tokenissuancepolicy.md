---
title: "tokenIssuancePolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# tokenIssuancePolicy resource type


Namespace: microsoft.graph




Inherits from [stsPolicy](../resources/stspolicy.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get tokenIssuancePolicy](../api/tokenissuancepolicy-get.md)|[tokenIssuancePolicy](../resources/tokenissuancepolicy.md)|Read properties and relationships of the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.|
|[Update tokenIssuancePolicy](../api/tokenissuancepolicy-update.md)|[tokenIssuancePolicy](../resources/tokenissuancepolicy.md)|Update the properties of a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.|
|[List appliesTo](../api/tokenissuancepolicy-list-appliesto.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the appliesTo navigation property.|
|[Create appliesTo](../api/tokenissuancepolicy-post-appliesto.md)|[directoryObject](../resources/directoryobject.md)|Create appliesTo by posting to the appliesTo collection.|

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

