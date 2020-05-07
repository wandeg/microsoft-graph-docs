---
title: "applicationTemplate resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# applicationTemplate resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List applicationTemplates](../api/applicationtemplate-list.md)|[applicationTemplate](../resources/applicationtemplate.md) collection|Get a list of the [applicationTemplate](../resources/applicationtemplate.md) objects and their properties.|
|[Get applicationTemplate](../api/applicationtemplate-get.md)|[applicationTemplate](../resources/applicationtemplate.md)|Read the properties and relationships of an [applicationTemplate](../resources/applicationtemplate.md) object.|
|[Create applicationTemplate](../api/applicationtemplate-post-applicationtemplates.md)|[applicationTemplate](../resources/applicationtemplate.md)|Create a new [applicationTemplate](../resources/applicationtemplate.md) object.|
|[Delete applicationTemplate](../api/applicationtemplate-delete.md)|None|Deletes an [applicationTemplate](../resources/applicationtemplate.md) object.|
|[Update applicationTemplate](../api/applicationtemplate-update.md)|[applicationTemplate](../resources/applicationtemplate.md)|Update the properties of an [applicationTemplate](../resources/applicationtemplate.md) object.|
|[instantiate](../api/applicationtemplate-instantiate.md)|[applicationServicePrincipal](../resources/applicationserviceprincipal.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|categories|String collection|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|homePageUrl|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|logoUrl|String|**TODO: Add Description**|
|publisher|String|**TODO: Add Description**|
|supportedProvisioningTypes|String collection|**TODO: Add Description**|
|supportedSingleSignOnModes|String collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.applicationTemplate",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applicationTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "homePageUrl": "String",
  "supportedSingleSignOnModes": [
    "String"
  ],
  "supportedProvisioningTypes": [
    "String"
  ],
  "logoUrl": "String",
  "categories": [
    "String"
  ],
  "publisher": "String",
  "description": "String"
}
```

