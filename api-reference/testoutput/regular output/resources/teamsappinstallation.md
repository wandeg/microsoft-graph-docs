---
title: "teamsAppInstallation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# teamsAppInstallation resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List teamsAppInstallations](../api/teamsappinstallation-list.md)|[teamsAppInstallation](../resources/teamsappinstallation.md) collection|List properties and relationships of the [teamsAppInstallation](../resources/teamsappinstallation.md) objects.|
|[Get teamsAppInstallation](../api/teamsappinstallation-get.md)|[teamsAppInstallation](../resources/teamsappinstallation.md)|Read properties and relationships of the [teamsAppInstallation](../resources/teamsappinstallation.md) object.|
|[Create teamsAppInstallation](../api/teamsappinstallation-create.md)|[teamsAppInstallation](../resources/teamsappinstallation.md)|Create a new [teamsAppInstallation](../resources/teamsappinstallation.md) object.|
|[Delete teamsAppInstallation](../api/teamsappinstallation-delete.md)|None|Deletes a [teamsAppInstallation](../resources/teamsappinstallation.md).|
|[Update teamsAppInstallation](../api/teamsappinstallation-update.md)|[teamsAppInstallation](../resources/teamsappinstallation.md)|Update the properties of a [teamsAppInstallation](../resources/teamsappinstallation.md) object.|
|[upgrade](../api/teamsappinstallation-upgrade.md)|None||
|[Get teamsApp](../api/teamsapp-get.md)|[teamsApp](../resources/teamsapp.md)|Read properties and relationships of the [teamsApp](../resources/teamsapp.md) object.|
|[Get teamsAppDefinition](../api/teamsappdefinition-get.md)|[teamsAppDefinition](../resources/teamsappdefinition.md)|Read properties and relationships of the [teamsAppDefinition](../resources/teamsappdefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|teamsApp|[teamsApp](../resources/teamsapp.md)||
|teamsAppDefinition|[teamsAppDefinition](../resources/teamsappdefinition.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsAppInstallation",
  "id": "String (identifier)"
}
```

