---
title: "teamwork resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# teamwork resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get teamwork](../api/teamwork-get.md)|[teamwork](../resources/teamwork.md)|Read properties and relationships of the [teamwork](../resources/teamwork.md) object.|
|[Update teamwork](../api/teamwork-update.md)|[teamwork](../resources/teamwork.md)|Update the properties of a [teamwork](../resources/teamwork.md) object.|
|[List workforceIntegrations](../api/teamwork-list-workforceintegrations.md)|[workforceIntegration](../resources/workforceintegration.md) collection|Get the workforceIntegrations from the workforceIntegrations navigation property.|
|[Add workforceIntegrations](../api/teamwork-post-workforceintegrations.md)|[workforceIntegration](../resources/workforceintegration.md)|Add workforceIntegrations by posting to the workforceIntegrations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|workforceIntegrations|[workforceIntegration](../resources/workforceintegration.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamwork",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamwork",
  "id": "String (identifier)"
}
```

