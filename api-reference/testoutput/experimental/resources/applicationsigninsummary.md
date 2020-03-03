---
title: "applicationSignInSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# applicationSignInSummary resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List applicationSignInSummaries](../api/applicationsigninsummary-list.md)|[applicationSignInSummary](../resources/applicationSignInSummary.md) collection|List properties and relationships of the [applicationSignInSummary](../resources/applicationsigninsummary.md) objects.|
|[Get applicationSignInSummary](../api/applicationsigninsummary-get.md)|[applicationSignInSummary](../resources/applicationSignInSummary.md)|Read properties and relationships of the [applicationSignInSummary](../resources/applicationsigninsummary.md) object.|
|[Create applicationSignInSummary](../api/applicationsigninsummary-create.md)|[applicationSignInSummary](../resources/applicationSignInSummary.md)|Create a new [applicationSignInSummary](../resources/applicationsigninsummary.md) object.|
|[Delete applicationSignInSummary](../api/applicationsigninsummary-delete.md)|None|Deletes a [applicationSignInSummary](../resources/applicationsigninsummary.md).|
|[Update applicationSignInSummary](../api/applicationsigninsummary-update.md)|[applicationSignInSummary](../resources/applicationSignInSummary.md)|Update the properties of a [applicationSignInSummary](../resources/applicationsigninsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appDisplayName|String||
|failedSignInCount|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|successfulSignInCount|Int64||
|successPercentage|Double||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
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
  "successfulSignInCount": 1024,
  "failedSignInCount": 1024,
  "successPercentage": "Double"
}
```

