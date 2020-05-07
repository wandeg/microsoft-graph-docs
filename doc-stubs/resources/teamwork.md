---
title: "teamwork resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# teamwork resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[Get teamwork](../api/teamwork-get.md)|[teamwork](../resources/teamwork.md)|Read the properties and relationships of a [teamwork](../resources/teamwork.md) object.|
|[Update teamwork](../api/teamwork-update.md)|[teamwork](../resources/teamwork.md)|Update the properties of a [teamwork](../resources/teamwork.md) object.|
|[generateActivityNotification](../api/teamwork-generateactivitynotification.md)|None|**TODO: Add Description**|
|[List workforceIntegrations](../api/teamwork-list-workforceintegrations.md)|[workforceIntegration](../resources/workforceintegration.md) collection|Get the workforceIntegrations from the workforceIntegrations navigation property.|
|[Create workforceIntegrations](../api/teamwork-post-workforceintegrations.md)|[workforceIntegration](../resources/workforceintegration.md)|Create a new workforceIntegrations object.|
|[Delete workforceIntegrations](../api/teamwork-delete-workforceintegrations.md)|None|Delete a [workforceIntegration](../resources/workforceintegration.md) object.|
|[Update workforceIntegrations](../api/teamwork-update-workforceintegrations.md)|[workforceIntegration](../resources/workforceintegration.md)|Update the properties of a workforceIntegrations object.|
|[Get workforceIntegration](../api/workforceintegration-get.md)|[workforceIntegration](../resources/workforceintegration.md)|Read the properties and relationships of a [workforceIntegration](../resources/workforceintegration.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|workforceIntegrations|[workforceIntegration](../resources/workforceintegration.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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

