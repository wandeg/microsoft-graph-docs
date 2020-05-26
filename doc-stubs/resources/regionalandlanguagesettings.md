---
title: "regionalAndLanguageSettings resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# regionalAndLanguageSettings resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List regionalAndLanguageSettings](../api/usersettings-list-regionalandlanguagesettings.md)|[regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) collection|Get the regionalAndLanguageSettings from the regionalAndLanguageSettings navigation property.|
|[Create regionalAndLanguageSettings](../api/usersettings-post-regionalandlanguagesettings.md)|[regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md)|Create a new regionalAndLanguageSettings object.|
|[Update regionalAndLanguageSettings](../api/usersettings-update-regionalandlanguagesettings.md)|[regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md)|Update the properties of a regionalAndLanguageSettings object.|
|[Get regionalAndLanguageSettings](../api/usersettings-get-regionalandlanguagesettings.md)|[regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md)|Read the properties and relationships of a [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) object.|
|[Delete regionalAndLanguageSettings](../api/usersettings-delete-regionalandlanguagesettings.md)|None|Delete a [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) object.|
|[List regionalAndLanguageSettings](../api/regionalandlanguagesettings-list.md)|[regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) collection|Get a list of the [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) objects and their properties.|
|[Create regionalAndLanguageSettings](../api/regionalandlanguagesettings-create.md)|[regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md)|Create a new [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) object.|
|[Get regionalAndLanguageSettings](../api/regionalandlanguagesettings-get.md)|[regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md)|Read the properties and relationships of a [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) object.|
|[Update regionalAndLanguageSettings](../api/regionalandlanguagesettings-update.md)|[regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md)|Update the properties of a [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) object.|
|[Delete regionalAndLanguageSettings](../api/regionalandlanguagesettings-delete.md)|None|Deletes a [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|authoringLanguages|[localeInfo](../resources/localeinfo.md) collection|**TODO: Add Description**|
|defaultDisplayLanguage|[localeInfo](../resources/localeinfo.md)|**TODO: Add Description**|
|defaultRegionalFormat|[localeInfo](../resources/localeinfo.md)|**TODO: Add Description**|
|defaultSpeechInputLanguage|[localeInfo](../resources/localeinfo.md)|**TODO: Add Description**|
|defaultTranslationLanguage|[localeInfo](../resources/localeinfo.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|regionalFormatOverrides|[regionalFormatOverrides](../resources/regionalformatoverrides.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.regionalAndLanguageSettings",
  "id": "String (identifier)",
  "defaultDisplayLanguage": {
    "@odata.type": "microsoft.graph.localeInfo"
  },
  "authoringLanguages": [
    {
      "@odata.type": "microsoft.graph.localeInfo"
    }
  ],
  "defaultTranslationLanguage": {
    "@odata.type": "microsoft.graph.localeInfo"
  },
  "defaultSpeechInputLanguage": {
    "@odata.type": "microsoft.graph.localeInfo"
  },
  "defaultRegionalFormat": {
    "@odata.type": "microsoft.graph.localeInfo"
  },
  "regionalFormatOverrides": {
    "@odata.type": "microsoft.graph.regionalFormatOverrides"
  }
}
```

