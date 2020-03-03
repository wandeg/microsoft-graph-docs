---
title: "groupPolicyDefinition resource type"
description: "The entity describes all of the information about a single group policy."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# groupPolicyDefinition resource type

The entity describes all of the information about a single group policy.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get groupPolicyDefinition](../api/grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/groupPolicyDefinition.md)|Read properties and relationships of the [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|
|[Delete groupPolicyDefinition](../api/grouppolicydefinition-delete.md)|None|Deletes a [groupPolicyDefinition](../resources/grouppolicydefinition.md).|
|[Update groupPolicyDefinition](../api/grouppolicydefinition-update.md)|[groupPolicyDefinition](../resources/groupPolicyDefinition.md)|Update the properties of a [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|
|[Get groupPolicyDefinitionFile](../api/grouppolicydefinitionfile-get.md)|[groupPolicyDefinitionFile](../resources/groupPolicyDefinitionFile.md)|Read properties and relationships of the [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) object.|
|[List presentations](../api/grouppolicydefinition-list-presentations.md)|[groupPolicyPresentation](../resources/groupPolicyPresentation.md) collection|Get the groupPolicyPresentations from the presentations navigation property.|
|[Add presentations](../api/grouppolicydefinition-post-presentations.md)|[groupPolicyPresentation](../resources/groupPolicyPresentation.md)|Add presentations by posting to the presentations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|categoryPath|String|The localized full category path for the policy.|
|classType|Enumeration|Identifies the type of groups the policy can be applied to. Possible values are: `user`, `machine`.|
|displayName|String|The localized policy name.|
|explainText|String|The localized explanation or help text associated with the policy. The default value is empty.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified.|
|policyType|Enumeration|Specifies the type of group policy. Possible values are: `admxBacked`, `admxIngested`.|
|supportedOn|String|Localized string used to specify what operating system or application version is affected by the policy.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definitionFile|[groupPolicyDefinitionFile](../resources/groupPolicyDefinitionFile.md)|The group policy file associated with the definition.|
|presentations|[groupPolicyPresentation](../resources/groupPolicyPresentation.md) collection|The group policy presentations associated with the definition.|

## JSON Representation
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
  "lastModifiedDateTime": "String (timestamp)"
}
```

