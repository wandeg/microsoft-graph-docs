---
title: "applicationSignInSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# applicationSignInSummary resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List applicationSignInSummaries](../api/applicationsigninsummary-list.md)|[applicationSignInSummary](../resources/applicationsigninsummary.md) collection|Get a list of the [applicationSignInSummary](../resources/applicationsigninsummary.md) objects and their properties.|
|[Create applicationSignInSummary](../api/applicationsigninsummary-create.md)|[applicationSignInSummary](../resources/applicationsigninsummary.md)|Create a new [applicationSignInSummary](../resources/applicationsigninsummary.md) object.|
|[Get applicationSignInSummary](../api/applicationsigninsummary-get.md)|[applicationSignInSummary](../resources/applicationsigninsummary.md)|Read the properties and relationships of an [applicationSignInSummary](../resources/applicationsigninsummary.md) object.|
|[Update applicationSignInSummary](../api/applicationsigninsummary-update.md)|[applicationSignInSummary](../resources/applicationsigninsummary.md)|Update the properties of an [applicationSignInSummary](../resources/applicationsigninsummary.md) object.|
|[Delete applicationSignInSummary](../api/applicationsigninsummary-delete.md)|None|Deletes an [applicationSignInSummary](../resources/applicationsigninsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appDisplayName|String|**TODO: Add Description**|
|failedSignInCount|Int64|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|successfulSignInCount|Int64|**TODO: Add Description**|
|successPercentage|Double|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.applicationSignInSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applicationSignInSummary",
  "id": "String (identifier)",
  "appDisplayName": "String",
  "successfulSignInCount": "Integer",
  "failedSignInCount": "Integer",
  "successPercentage": "Double"
}
```

