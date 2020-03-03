---
title: "groupPolicyDefinitionFile resource type"
description: "The entity represents an ADMX (Administrative Template) XML file. The ADMX file contains a collection of group policy definitions and their locations by category path. The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# groupPolicyDefinitionFile resource type

The entity represents an ADMX (Administrative Template) XML file. The ADMX file contains a collection of group policy definitions and their locations by category path. The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get groupPolicyDefinitionFile](../api/grouppolicydefinitionfile-get.md)|[groupPolicyDefinitionFile](../resources/groupPolicyDefinitionFile.md)|Read properties and relationships of the [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) object.|
|[Delete groupPolicyDefinitionFile](../api/grouppolicydefinitionfile-delete.md)|None|Deletes a [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md).|
|[Update groupPolicyDefinitionFile](../api/grouppolicydefinitionfile-update.md)|[groupPolicyDefinitionFile](../resources/groupPolicyDefinitionFile.md)|Update the properties of a [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) object.|
|[List definitions](../api/grouppolicydefinitionfile-list-definitions.md)|[groupPolicyDefinition](../resources/groupPolicyDefinition.md) collection|Get the groupPolicyDefinitions from the definitions navigation property.|
|[Create definitions](../api/grouppolicydefinitionfile-post-definitions.md)|[groupPolicyDefinition](../resources/groupPolicyDefinition.md)|Create definitions by posting to the definitions collection.|
|[List groupPolicyDefinitionFiles](../api/intune-devices-devicemanagement-list-grouppolicydefinitionfiles.md)|[groupPolicyDefinitionFile](../resources/groupPolicyDefinitionFile.md) collection|Get the groupPolicyDefinitionFiles from the groupPolicyDefinitionFiles navigation property.|
|[Add groupPolicyDefinitionFiles](../api/intune-devices-devicemanagement-post-grouppolicydefinitionfiles.md)|[groupPolicyDefinitionFile](../resources/groupPolicyDefinitionFile.md)|Add groupPolicyDefinitionFiles by posting to the groupPolicyDefinitionFiles collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|The localized description of the policy settings in the ADMX file. The default value is empty.|
|displayName|String|The localized friendly name of the ADMX file.|
|id|String| Inherited from [entity](../resources/entity.md)|
|languageCodes|String collection|The supported language codes for the ADMX file.|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified.|
|policyType|Enumeration|Specifies the type of group policy. Possible values are: `admxBacked`, `admxIngested`.|
|revision|String|The revision version associated with the file.|
|targetNamespace|String|Specifies the URI used to identify the namespace within the ADMX file.|
|targetPrefix|String|Specifies the logical name that refers to the namespace within the ADMX file.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definitions|[groupPolicyDefinition](../resources/groupPolicyDefinition.md) collection|The group policy definitions associated with the file.|

## JSON Representation
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

