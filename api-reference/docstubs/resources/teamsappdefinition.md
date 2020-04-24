---
title: "teamsAppDefinition resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# teamsAppDefinition resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get teamsAppDefinition](../api/teamsappdefinition-get.md)|[teamsAppDefinition](../resources/teamsappdefinition.md)|Read the properties and relationships of a [teamsAppDefinition](../resources/teamsappdefinition.md) object.|
|[Update teamsAppDefinition](../api/teamsappdefinition-update.md)|[teamsAppDefinition](../resources/teamsappdefinition.md)|Update the properties of a [teamsAppDefinition](../resources/teamsappdefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|teamsAppId|String|**TODO: Add Description**|
|version|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsAppDefinition",
  "id": "String (identifier)",
  "teamsAppId": "String",
  "displayName": "String",
  "version": "String"
}
```

