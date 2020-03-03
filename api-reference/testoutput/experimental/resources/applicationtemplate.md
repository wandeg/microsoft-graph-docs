---
title: "applicationTemplate resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# applicationTemplate resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List applicationTemplates](../api/applicationtemplate-list.md)|[applicationTemplate](../resources/applicationTemplate.md) collection|List properties and relationships of the [applicationTemplate](../resources/applicationtemplate.md) objects.|
|[Get applicationTemplate](../api/applicationtemplate-get.md)|[applicationTemplate](../resources/applicationTemplate.md)|Read properties and relationships of the [applicationTemplate](../resources/applicationtemplate.md) object.|
|[Create applicationTemplate](../api/applicationtemplate-post-applicationtemplates.md)|[applicationTemplate](../resources/applicationTemplate.md)|Create a new [applicationTemplate](../resources/applicationtemplate.md) object.|
|[Delete applicationTemplate](../api/applicationtemplate-delete.md)|None|Deletes a [applicationTemplate](../resources/applicationtemplate.md).|
|[Update applicationTemplate](../api/applicationtemplate-update.md)|[applicationTemplate](../resources/applicationTemplate.md)|Update the properties of a [applicationTemplate](../resources/applicationtemplate.md) object.|
|[instantiate](../api/applicationtemplate-instantiate.md)|[applicationServicePrincipal](../resources/applicationServicePrincipal.md)||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|categories|String collection||
|description|String||
|displayName|String||
|homePageUrl|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|logoUrl|String||
|publisher|String||
|supportedProvisioningTypes|String collection||
|supportedSingleSignOnModes|String collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
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

