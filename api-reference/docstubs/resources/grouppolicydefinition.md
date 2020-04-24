---
title: "groupPolicyDefinition resource type"
description: "The entity describes all of the information about a single group policy."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# groupPolicyDefinition resource type


Namespace: microsoft.graph

The entity describes all of the information about a single group policy.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get groupPolicyDefinition](../api/grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Read the properties and relationships of a [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|
|[Update groupPolicyDefinition](../api/grouppolicydefinition-update.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Update the properties of a [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|
|[List definitionFile](../api/grouppolicydefinition-list-definitionfile.md)|[groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) collection|Get the groupPolicyDefinitionFiles from the definitionFile navigation property.|
|[Add definitionFile](../api/grouppolicydefinition-post-definitionfile.md)|[groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|Add definitionFile by posting to the definitionFile collection.|
|[Remove definitionFile](../api/grouppolicydefinition-delete-definitionfile.md)|None|Remove a [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) object.|
|[List category](../api/grouppolicydefinition-list-category.md)|[groupPolicyCategory](../resources/grouppolicycategory.md) collection|Get the groupPolicyCategories from the category navigation property.|
|[Add category](../api/grouppolicydefinition-post-category.md)|[groupPolicyCategory](../resources/grouppolicycategory.md)|Add category by posting to the category collection.|
|[Remove category](../api/grouppolicydefinition-delete-category.md)|None|Remove a [groupPolicyCategory](../resources/grouppolicycategory.md) object.|
|[List presentations](../api/grouppolicydefinition-list-presentations.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md) collection|Get the groupPolicyPresentations from the presentations navigation property.|
|[Create presentations](../api/grouppolicydefinition-post-presentations.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|Create a new presentations object.|
|[Delete presentations](../api/grouppolicydefinition-delete-presentations.md)|None|Delete a [groupPolicyPresentation](../resources/grouppolicypresentation.md) object.|
|[Update presentations](../api/grouppolicydefinition-update-presentations.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|Update the properties of a presentations object.|
|[Get groupPolicyPresentation](../api/grouppolicypresentation-get.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|Read the properties and relationships of a [groupPolicyPresentation](../resources/grouppolicypresentation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|categoryPath|String|The localized full category path for the policy.|
|classType|groupPolicyDefinitionClassType|Identifies the type of groups the policy can be applied to. Possible values are: `user`, `machine`.|
|displayName|String|The localized policy name.|
|explainText|String|The localized explanation or help text associated with the policy. The default value is empty.|
|groupPolicyCategoryId|Guid|The category id of the parent category|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified.|
|policyType|groupPolicyType|Specifies the type of group policy. Possible values are: `admxBacked`, `admxIngested`.|
|supportedOn|String|Localized string used to specify what operating system or application version is affected by the policy.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|category|[groupPolicyCategory](../resources/grouppolicycategory.md)|The group policy category associated with the definition.|
|definitionFile|[groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|The group policy file associated with the definition.|
|presentations|[groupPolicyPresentation](../resources/grouppolicypresentation.md) collection|The group policy presentations associated with the definition.|

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

