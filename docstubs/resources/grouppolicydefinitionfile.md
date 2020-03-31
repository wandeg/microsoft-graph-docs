---
title: "groupPolicyDefinitionFile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupPolicyDefinitionFile resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get groupPolicyDefinitionFile](../api/grouppolicydefinitionfile-get.md)|[groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|Read properties and relationships of the [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) object.|
|[Update groupPolicyDefinitionFile](../api/grouppolicydefinitionfile-update.md)|[groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|Update the properties of a [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) object.|
|[List definitions](../api/grouppolicydefinitionfile-list-definitions.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md) collection|Get the groupPolicyDefinitions from the definitions navigation property.|
|[Create definitions](../api/grouppolicydefinitionfile-post-definitions.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Create definitions by posting to the definitions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|languageCodes|String collection||
|lastModifiedDateTime|DateTimeOffset||
|policyType|Enumeration| Possible values are: `admxBacked`, `admxIngested`.|
|revision|String||
|targetNamespace|String||
|targetPrefix|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definitions|[groupPolicyDefinition](../resources/grouppolicydefinition.md) collection||

## JSON representation
Here is a JSON representation of the resource.
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

