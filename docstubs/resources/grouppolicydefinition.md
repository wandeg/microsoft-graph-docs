---
title: "groupPolicyDefinition resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupPolicyDefinition resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get groupPolicyDefinition](../api/grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Read properties and relationships of the [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|
|[Update groupPolicyDefinition](../api/grouppolicydefinition-update.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Update the properties of a [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|
|[Get groupPolicyDefinitionFile](../api/grouppolicydefinitionfile-get.md)|[groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|Read properties and relationships of the [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) object.|
|[Get groupPolicyCategory](../api/grouppolicycategory-get.md)|[groupPolicyCategory](../resources/grouppolicycategory.md)|Read properties and relationships of the [groupPolicyCategory](../resources/grouppolicycategory.md) object.|
|[List presentations](../api/grouppolicydefinition-list-presentations.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md) collection|Get the groupPolicyPresentations from the presentations navigation property.|
|[Add presentations](../api/grouppolicydefinition-post-presentations.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|Add presentations by posting to the presentations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|categoryPath|String||
|classType|Enumeration| Possible values are: `user`, `machine`.|
|displayName|String||
|explainText|String||
|groupPolicyCategoryId|Guid||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|policyType|Enumeration| Possible values are: `admxBacked`, `admxIngested`.|
|supportedOn|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|category|[groupPolicyCategory](../resources/grouppolicycategory.md)||
|definitionFile|[groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)||
|presentations|[groupPolicyPresentation](../resources/grouppolicypresentation.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "id": "String (identifier)",
  "classType": "String",
  "displayName": "String",
  "explainText": "String",
  "categoryPath": "String",
  "supportedOn": "String",
  "policyType": "String",
  "groupPolicyCategoryId": "Guid",
  "lastModifiedDateTime": "String (timestamp)"
}
```

