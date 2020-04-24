---
title: "activityBasedTimeoutPolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# activityBasedTimeoutPolicy resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [stsPolicy](../resources/stspolicy.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get activityBasedTimeoutPolicy](../api/activitybasedtimeoutpolicy-get.md)|[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)|Read the properties and relationships of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.|
|[Update activityBasedTimeoutPolicy](../api/activitybasedtimeoutpolicy-update.md)|[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)|Update the properties of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.|
|[List appliesTo](../api/activitybasedtimeoutpolicy-list-appliesto.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the appliesTo navigation property.|
|[Add appliesTo](../api/activitybasedtimeoutpolicy-post-appliesto.md)|[directoryObject](../resources/directoryobject.md)|Add appliesTo by posting to the appliesTo collection.|
|[Remove appliesTo](../api/activitybasedtimeoutpolicy-delete-appliesto.md)|None|Remove an [directoryObject](../resources/directoryobject.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|definition|String collection|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md)|
|description|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|displayName|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isOrganizationDefault|Boolean|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliesTo|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md)|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy",
  "baseType": "microsoft.graph.stsPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.activityBasedTimeoutPolicy",
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "definition": [
    "String"
  ],
  "isOrganizationDefault": true
}
```

