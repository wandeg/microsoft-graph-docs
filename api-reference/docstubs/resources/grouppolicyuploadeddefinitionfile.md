---
title: "groupPolicyUploadedDefinitionFile resource type"
description: "The entity represents an ADMX (Administrative Template) XML file uploaded by Administrator. The ADMX file contains a collection of group policy definitions and their locations by category path. The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# groupPolicyUploadedDefinitionFile resource type


Namespace: microsoft.graph

The entity represents an ADMX (Administrative Template) XML file uploaded by Administrator. The ADMX file contains a collection of group policy definitions and their locations by category path. The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.


Inherits from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get groupPolicyUploadedDefinitionFile](../api/grouppolicyuploadeddefinitionfile-get.md)|[groupPolicyUploadedDefinitionFile](../resources/grouppolicyuploadeddefinitionfile.md)|Read the properties and relationships of a [groupPolicyUploadedDefinitionFile](../resources/grouppolicyuploadeddefinitionfile.md) object.|
|[Update groupPolicyUploadedDefinitionFile](../api/grouppolicyuploadeddefinitionfile-update.md)|[groupPolicyUploadedDefinitionFile](../resources/grouppolicyuploadeddefinitionfile.md)|Update the properties of a [groupPolicyUploadedDefinitionFile](../resources/grouppolicyuploadeddefinitionfile.md) object.|
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
|content|Binary|The contents of the uploaded ADMX file.|
|defaultLanguageCode|String|The default language of the uploaded ADMX file.|
|description|String|The localized description of the policy settings in the ADMX file. The default value is empty. Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|displayName|String|The localized friendly name of the ADMX file. Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|fileName|String|The file name of the uploaded ADML file.|
|groupPolicyUploadedLanguageFiles|[groupPolicyUploadedLanguageFile](../resources/grouppolicyuploadedlanguagefile.md) collection|The list of ADML files associated with the uploaded ADMX file.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|languageCodes|String collection|The supported language codes for the ADMX file. Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified. Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|policyType|groupPolicyType|Specifies the type of group policy. Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md). Possible values are: `admxBacked`, `admxIngested`.|
|revision|String|The revision version associated with the file. Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|status|groupPolicyUploadedDefinitionFileStatus|The upload status of the uploaded ADMX file. Possible values are: `none`, `uploadInProgress`, `available`, `assigned`, `removalInProgress`, `uploadFailed`, `removalFailed`.|
|targetNamespace|String|Specifies the URI used to identify the namespace within the ADMX file. Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|targetPrefix|String|Specifies the logical name that refers to the namespace within the ADMX file. Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|uploadDateTime|DateTimeOffset|The uploaded time of the uploaded ADMX file.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definitions|[groupPolicyDefinition](../resources/grouppolicydefinition.md) collection|The group policy definitions associated with the file. Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|groupPolicyOperations|[groupPolicyOperation](../resources/grouppolicyoperation.md) collection|The list of operations on the uploaded ADMX file.|

## JSON representation
Here is a JSON representation of the resource.
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
  "content": "binary",
  "uploadDateTime": "String (timestamp)",
  "defaultLanguageCode": "String",
  "groupPolicyUploadedLanguageFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile",
      "languageCode": "String",
      "id": "String"
    }
  ]
}
```

