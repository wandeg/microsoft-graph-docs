---
title: "groupPolicyUploadedDefinitionFile resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# groupPolicyUploadedDefinitionFile resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[addLanguageFiles](../api/grouppolicyuploadeddefinitionfile-addlanguagefiles.md)|None|**TODO: Add Description**|
|[removeLanguageFiles](../api/grouppolicyuploadeddefinitionfile-removelanguagefiles.md)|None|**TODO: Add Description**|
|[updateLanguageFiles](../api/grouppolicyuploadeddefinitionfile-updatelanguagefiles.md)|None|**TODO: Add Description**|
|[uploadNewVersion](../api/grouppolicyuploadeddefinitionfile-uploadnewversion.md)|None|**TODO: Add Description**|
|[remove](../api/grouppolicyuploadeddefinitionfile-remove.md)|None|**TODO: Add Description**|
|[List definitions](../api/grouppolicyuploadeddefinitionfile-list-definitions.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md) collection|Get the groupPolicyDefinitions from the definitions navigation property.|
|[Add definitions](../api/grouppolicyuploadeddefinitionfile-post-definitions.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Add definitions by posting to the definitions collection.|
|[Remove definitions](../api/grouppolicyuploadeddefinitionfile-delete-definitions.md)|None|Remove a [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|
|[List groupPolicyOperations](../api/grouppolicyuploadeddefinitionfile-list-grouppolicyoperations.md)|[groupPolicyOperation](../resources/grouppolicyoperation.md) collection|Get the groupPolicyOperations from the groupPolicyOperations navigation property.|
|[Add groupPolicyOperations](../api/grouppolicyuploadeddefinitionfile-post-grouppolicyoperations.md)|[groupPolicyOperation](../resources/grouppolicyoperation.md)|Add groupPolicyOperations by posting to the groupPolicyOperations collection.|
|[Remove groupPolicyOperations](../api/grouppolicyuploadeddefinitionfile-delete-grouppolicyoperations.md)|None|Remove a [groupPolicyOperation](../resources/grouppolicyoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|Binary|**TODO: Add Description**|
|defaultLanguageCode|String|**TODO: Add Description**|
|description|String|**TODO: Add Description** Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|displayName|String|**TODO: Add Description** Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|fileName|String|**TODO: Add Description**|
|groupPolicyUploadedLanguageFiles|[groupPolicyUploadedLanguageFile](../resources/grouppolicyuploadedlanguagefile.md) collection|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|languageCodes|String collection|**TODO: Add Description** Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|policyType|groupPolicyType|**TODO: Add Description** Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md). Possible values are: `admxBacked`, `admxIngested`.|
|revision|String|**TODO: Add Description** Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|status|groupPolicyUploadedDefinitionFileStatus|**TODO: Add Description**. Possible values are: `none`, `uploadInProgress`, `available`, `assigned`, `removalInProgress`, `uploadFailed`, `removalFailed`.|
|targetNamespace|String|**TODO: Add Description** Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|targetPrefix|String|**TODO: Add Description** Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|uploadDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definitions|[groupPolicyDefinition](../resources/grouppolicydefinition.md) collection|**TODO: Add Description** Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|groupPolicyOperations|[groupPolicyOperation](../resources/grouppolicyoperation.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyUploadedDefinitionFile",
  "baseType": "microsoft.graph.groupPolicyDefinitionFile",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinitionFile",
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
  "lastModifiedDateTime": "String (timestamp)",
  "fileName": "String",
  "status": "String",
  "content": "Binary",
  "uploadDateTime": "String (timestamp)",
  "defaultLanguageCode": "String",
  "groupPolicyUploadedLanguageFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile"
    }
  ]
}
```

