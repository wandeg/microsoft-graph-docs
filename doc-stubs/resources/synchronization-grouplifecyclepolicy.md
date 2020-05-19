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
|[List groupLifecyclePolicies](../api/group-list-grouplifecyclepolicies.md)|[groupLifecyclePolicy](../resources/synchronization-grouplifecyclepolicy.md) collection|Get the groupLifecyclePolicies from the groupLifecyclePolicies navigation property.|
|[Create groupLifecyclePolicies](../api/group-post-grouplifecyclepolicies.md)|[groupLifecyclePolicy](../resources/synchronization-grouplifecyclepolicy.md)|Create a new groupLifecyclePolicies object.|
|[Delete groupLifecyclePolicies](../api/group-delete-grouplifecyclepolicies.md)|None|Delete a [groupLifecyclePolicy](../resources/synchronization-grouplifecyclepolicy.md) object.|
|[Update groupLifecyclePolicies](../api/group-update-grouplifecyclepolicies.md)|[groupLifecyclePolicy](../resources/synchronization-grouplifecyclepolicy.md)|Update the properties of a groupLifecyclePolicies object.|
|[Get groupLifecyclePolicies](../api/group-get-grouplifecyclepolicy.md)|[groupLifecyclePolicy](../resources/synchronization-grouplifecyclepolicy.md)|Read the properties and relationships of a [groupLifecyclePolicy](../resources/synchronization-grouplifecyclepolicy.md) object.|
|[List groupLifecyclePolicies](../api/synchronization-grouplifecyclepolicy-list.md)|[groupLifecyclePolicy](../resources/synchronization-grouplifecyclepolicy.md) collection|Get a list of the [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects and their properties.|
|[Get groupLifecyclePolicy](../api/synchronization-grouplifecyclepolicy-get.md)|[groupLifecyclePolicy](../resources/synchronization-grouplifecyclepolicy.md)|Read the properties and relationships of a [groupLifecyclePolicy](../resources/synchronization-grouplifecyclepolicy.md) object.|
|[Create groupLifecyclePolicy](../api/synchronization-grouplifecyclepolicy-post-grouplifecyclepolicies.md)|[groupLifecyclePolicy](../resources/synchronization-grouplifecyclepolicy.md)|Create a new [groupLifecyclePolicy](../resources/synchronization-grouplifecyclepolicy.md) object.|
|[Delete groupLifecyclePolicy](../api/synchronization-grouplifecyclepolicy-delete.md)|None|Deletes a [groupLifecyclePolicy](../resources/synchronization-grouplifecyclepolicy.md) object.|
|[Update groupLifecyclePolicy](../api/synchronization-grouplifecyclepolicy-update.md)|[groupLifecyclePolicy](../resources/synchronization-grouplifecyclepolicy.md)|Update the properties of a [groupLifecyclePolicy](../resources/synchronization-grouplifecyclepolicy.md) object.|
|[addGroup](../api/synchronization-grouplifecyclepolicy-addgroup.md)|Boolean|**TODO: Add Description**|
|[removeGroup](../api/synchronization-grouplifecyclepolicy-removegroup.md)|Boolean|**TODO: Add Description**|

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

