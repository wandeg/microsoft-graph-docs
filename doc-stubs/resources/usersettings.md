---
title: "userSettings resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userSettings resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List userSettings](../api/usersettings-list.md)|[userSettings](../resources/usersettings.md) collection|Get a list of the [userSettings](../resources/usersettings.md) objects and their properties.|
|[Create userSettings](../api/usersettings-create.md)|[userSettings](../resources/usersettings.md)|Create a new [userSettings](../resources/usersettings.md) object.|
|[Get userSettings](../api/usersettings-get.md)|[userSettings](../resources/usersettings.md)|Read the properties and relationships of a [userSettings](../resources/usersettings.md) object.|
|[Update userSettings](../api/usersettings-update.md)|[userSettings](../resources/usersettings.md)|Update the properties of a [userSettings](../resources/usersettings.md) object.|
|[Delete userSettings](../api/usersettings-delete.md)|None|Deletes a [userSettings](../resources/usersettings.md) object.|
|[List regionalAndLanguageSettings](../api/usersettings-list-regionalandlanguagesettings.md)|[regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) collection|Get the regionalAndLanguageSettings from the regionalAndLanguageSettings navigation property.|
|[Create regionalAndLanguageSettings](../api/usersettings-post-regionalandlanguagesettings.md)|[regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md)|Create a new regionalAndLanguageSettings object.|
|[Get regionalAndLanguageSettings](../api/usersettings-get-regionalandlanguagesettings.md)|[regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md)|Read the properties and relationships of a [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) object.|
|[Update regionalAndLanguageSettings](../api/usersettings-update-regionalandlanguagesettings.md)|[regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md)|Update the properties of a regionalAndLanguageSettings object.|
|[Delete regionalAndLanguageSettings](../api/usersettings-delete-regionalandlanguagesettings.md)|None|Delete a [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|contributionToContentDiscoveryAsOrganizationDisabled|Boolean|**TODO: Add Description**|
|contributionToContentDiscoveryDisabled|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|regionalAndLanguageSettings|[regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md)|**TODO: Add Description**|
|shiftPreferences|[shiftPreferences](../resources/shiftpreferences.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userSettings",
  "id": "String (identifier)",
  "contributionToContentDiscoveryDisabled": "Boolean",
  "contributionToContentDiscoveryAsOrganizationDisabled": "Boolean"
}
```

