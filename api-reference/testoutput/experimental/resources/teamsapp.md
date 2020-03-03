---
title: "teamsApp resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# teamsApp resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List teamsApps](../api/teamsapp-list.md)|[teamsApp](../resources/teamsapp.md) collection|List properties and relationships of the [teamsApp](../resources/teamsapp.md) objects.|
|[Get teamsApp](../api/teamsapp-get.md)|[teamsApp](../resources/teamsapp.md)|Read properties and relationships of the [teamsApp](../resources/teamsapp.md) object.|
|[Create teamsApp](../api/teamsapp-create.md)|[teamsApp](../resources/teamsapp.md)|Create a new [teamsApp](../resources/teamsapp.md) object.|
|[Delete teamsApp](../api/teamsapp-delete.md)|None|Deletes a [teamsApp](../resources/teamsapp.md).|
|[Update teamsApp](../api/teamsapp-update.md)|[teamsApp](../resources/teamsapp.md)|Update the properties of a [teamsApp](../resources/teamsapp.md) object.|
|[List appDefinitions](../api/teamsapp-list-appdefinitions.md)|[teamsAppDefinition](../resources/teamsappdefinition.md) collection|Get the teamsAppDefinitions from the appDefinitions navigation property.|
|[Create appDefinitions](../api/teamsapp-post-appdefinitions.md)|[teamsAppDefinition](../resources/teamsappdefinition.md)|Create appDefinitions by posting to the appDefinitions collection.|
|[List teamsApps](../api/appcatalogs-list-teamsapps.md)|[teamsApp](../resources/teamsapp.md) collection|Get the teamsApps from the teamsApps navigation property.|
|[Add teamsApps](../api/appcatalogs-post-teamsapps.md)|[teamsApp](../resources/teamsapp.md)|Add teamsApps by posting to the teamsApps collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|distributionMethod|Enumeration|. Possible values are: `store`, `organization`, `sideloaded`, `unknownFutureValue`.|
|externalId|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appDefinitions|[teamsAppDefinition](../resources/teamsappdefinition.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsApp",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsApp",
  "id": "String (identifier)",
  "externalId": "String",
  "name": "String",
  "displayName": "String",
  "distributionMethod": "String"
}
```

