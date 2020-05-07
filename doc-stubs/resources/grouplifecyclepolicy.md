---
title: "groupLifecyclePolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# groupLifecyclePolicy resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List groupLifecyclePolicies](../api/grouplifecyclepolicy-list.md)|[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) collection|Get a list of the [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects and their properties.|
|[Get groupLifecyclePolicy](../api/grouplifecyclepolicy-get.md)|[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)|Read the properties and relationships of a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.|
|[Create groupLifecyclePolicy](../api/grouplifecyclepolicy-post-grouplifecyclepolicies.md)|[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)|Create a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.|
|[Delete groupLifecyclePolicy](../api/grouplifecyclepolicy-delete.md)|None|Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.|
|[Update groupLifecyclePolicy](../api/grouplifecyclepolicy-update.md)|[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)|Update the properties of a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.|
|[addGroup](../api/grouplifecyclepolicy-addgroup.md)|Boolean|**TODO: Add Description**|
|[removeGroup](../api/grouplifecyclepolicy-removegroup.md)|Boolean|**TODO: Add Description**|
|[renewGroup](../api/grouplifecyclepolicy-renewgroup.md)|Boolean|**TODO: Add Description**|
|[List groupLifecyclePolicies](../api/group-list-grouplifecyclepolicies.md)|[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) collection|Get the groupLifecyclePolicies from the groupLifecyclePolicies navigation property.|
|[Create groupLifecyclePolicies](../api/group-post-grouplifecyclepolicies.md)|[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)|Create a new groupLifecyclePolicies object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|alternateNotificationEmails|String|**TODO: Add Description**|
|groupLifetimeInDays|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|managedGroupTypes|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupLifecyclePolicy",
  "id": "String (identifier)",
  "groupLifetimeInDays": "Integer",
  "managedGroupTypes": "String",
  "alternateNotificationEmails": "String"
}
```

