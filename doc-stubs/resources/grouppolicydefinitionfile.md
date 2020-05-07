---
title: "groupPolicyDefinitionFile resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# groupPolicyDefinitionFile resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List definitions](../api/grouppolicydefinitionfile-list-definitions.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md) collection|Get the groupPolicyDefinitions from the definitions navigation property.|
|[Add definitions](../api/grouppolicydefinitionfile-post-definitions.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Add definitions by posting to the definitions collection.|
|[Remove definitions](../api/grouppolicydefinitionfile-delete-definitions.md)|None|Remove a [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|
|[List definitionFile](../api/grouppolicycategory-list-definitionfile.md)|[groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) collection|Get the groupPolicyDefinitionFiles from the definitionFile navigation property.|
|[Add definitionFile](../api/grouppolicycategory-post-definitionfile.md)|[groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|Add definitionFile by posting to the definitionFile collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|languageCodes|String collection|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|policyType|groupPolicyType|**TODO: Add Description**. Possible values are: `admxBacked`, `admxIngested`.|
|revision|String|**TODO: Add Description**|
|targetNamespace|String|**TODO: Add Description**|
|targetPrefix|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definitions|[groupPolicyDefinition](../resources/grouppolicydefinition.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinitionFile",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "languageCodes": [
    "String"
  ],
  "targetPrefix": "String",
  "targetNamespace": "String",
  "policyType": "String",
  "revision": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

