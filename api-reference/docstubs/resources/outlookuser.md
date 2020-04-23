---
title: "outlookUser resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# outlookUser resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get outlookUser](../api/outlookuser-get.md)|[outlookUser](../resources/outlookuser.md)|Read the properties and relationships of an [outlookUser](../resources/outlookuser.md) object.|
|[Update outlookUser](../api/outlookuser-update.md)|[outlookUser](../resources/outlookuser.md)|Update the properties of an [outlookUser](../resources/outlookuser.md) object.|
|[supportedLanguages](../api/outlookuser-supportedlanguages.md)|[localeInfo](../resources/localeinfo.md) collection|**TODO: Add Description**|
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md)|[timeZoneInformation](../resources/timezoneinformation.md) collection|**TODO: Add Description**|
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md)|[timeZoneInformation](../resources/timezoneinformation.md) collection|**TODO: Add Description**|
|[List masterCategories](../api/outlookuser-list-mastercategories.md)|[outlookCategory](../resources/outlookcategory.md) collection|Get the outlookCategories from the masterCategories navigation property.|
|[Create masterCategories](../api/outlookuser-post-mastercategories.md)|[outlookCategory](../resources/outlookcategory.md)|Create a new masterCategories object.|
|[Delete masterCategories](../api/outlookuser-delete-mastercategories.md)|None|Delete a [outlookCategory](../resources/outlookcategory.md) object.|
|[Update masterCategories](../api/outlookuser-update-mastercategories.md)|[outlookCategory](../resources/outlookcategory.md)|Update the properties of a masterCategories object.|
|[Get outlookCategory](../api/outlookcategory-get.md)|[outlookCategory](../resources/outlookcategory.md)|Read the properties and relationships of an [outlookCategory](../resources/outlookcategory.md) object.|
|[List outlook](../api/user-list-outlook.md)|[outlookUser](../resources/outlookuser.md) collection|Get the outlookUsers from the outlook navigation property.|
|[Create outlook](../api/user-post-outlook.md)|[outlookUser](../resources/outlookuser.md)|Create a new outlook object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|masterCategories|[outlookCategory](../resources/outlookcategory.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.outlookUser",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outlookUser",
  "id": "String (identifier)"
}
```

