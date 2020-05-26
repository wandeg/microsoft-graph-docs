---
title: "connectorGroup resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# connectorGroup resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List connectorGroup](../api/application-list-connectorgroup.md)|[connectorGroup](../resources/connectorgroup.md) collection|Get the connectorGroups from the connectorGroup navigation property.|
|[Add connectorGroup](../api/application-post-connectorgroup.md)|[connectorGroup](../resources/connectorgroup.md)|Add connectorGroup by posting to the connectorGroup collection.|
|[Remove connectorGroup](../api/application-delete-connectorgroup.md)|None|Remove a [connectorGroup](../resources/connectorgroup.md) object.|
|[List connectorGroups](../api/connectorgroup-list.md)|[connectorGroup](../resources/connectorgroup.md) collection|Get a list of the [connectorGroup](../resources/connectorgroup.md) objects and their properties.|
|[Create connectorGroup](../api/connectorgroup-post-connectorgroups.md)|[connectorGroup](../resources/connectorgroup.md)|Create a new [connectorGroup](../resources/connectorgroup.md) object.|
|[Get connectorGroup](../api/connectorgroup-get.md)|[connectorGroup](../resources/connectorgroup.md)|Read the properties and relationships of a [connectorGroup](../resources/connectorgroup.md) object.|
|[Update connectorGroup](../api/connectorgroup-update.md)|[connectorGroup](../resources/connectorgroup.md)|Update the properties of a [connectorGroup](../resources/connectorgroup.md) object.|
|[Delete connectorGroup](../api/connectorgroup-delete.md)|None|Deletes a [connectorGroup](../resources/connectorgroup.md) object.|
|[List applications](../api/connectorgroup-list-applications.md)|[application](../resources/application.md) collection|Get the applications from the applications navigation property.|
|[Add applications](../api/connectorgroup-post-applications.md)|[application](../resources/application.md)|Add applications by posting to the applications collection.|
|[Remove applications](../api/connectorgroup-delete-applications.md)|None|Remove an [application](../resources/application.md) object.|
|[List members](../api/connectorgroup-list-members.md)|[connector](../resources/connector.md) collection|Get the connectors from the members navigation property.|
|[Add members](../api/connectorgroup-post-members.md)|[connector](../resources/connector.md)|Add members by posting to the members collection.|
|[Remove members](../api/connectorgroup-delete-members.md)|None|Remove a [connector](../resources/connector.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|connectorGroupType|connectorGroupType|**TODO: Add Description**. Possible values are: `applicationProxy`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isDefault|Boolean|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|region|connectorGroupRegion|**TODO: Add Description**. Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`, `unknownFutureValue`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|applications|[application](../resources/application.md) collection|**TODO: Add Description**|
|members|[connector](../resources/connector.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.connectorGroup",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.connectorGroup",
  "id": "String (identifier)",
  "name": "String",
  "connectorGroupType": "String",
  "isDefault": "Boolean",
  "region": "String"
}
```

