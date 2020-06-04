---
title: "authorizationPolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# authorizationPolicy resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [policyBase](../resources/policybase.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List authorizationPolicies](../api/authorizationpolicy-list.md)|[authorizationPolicy](../resources/authorizationpolicy.md) collection|Get a list of the [authorizationPolicy](../resources/authorizationpolicy.md) objects and their properties.|
|[Create authorizationPolicy](../api/authorizationpolicy-create.md)|[authorizationPolicy](../resources/authorizationpolicy.md)|Create a new [authorizationPolicy](../resources/authorizationpolicy.md) object.|
|[Get authorizationPolicy](../api/authorizationpolicy-get.md)|[authorizationPolicy](../resources/authorizationpolicy.md)|Read the properties and relationships of an [authorizationPolicy](../resources/authorizationpolicy.md) object.|
|[Update authorizationPolicy](../api/authorizationpolicy-update.md)|[authorizationPolicy](../resources/authorizationpolicy.md)|Update the properties of an [authorizationPolicy](../resources/authorizationpolicy.md) object.|
|[Delete authorizationPolicy](../api/authorizationpolicy-delete.md)|None|Deletes an [authorizationPolicy](../resources/authorizationpolicy.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|blockMsolPowerShell|Boolean|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|displayName|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|enabledPreviewFeatures|String collection|**TODO: Add Description**|
|guestUserRoleId|Guid|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|permissionGrantPolicyIdsAssignedToDefaultUserRole|String collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authorizationPolicy",
  "baseType": "microsoft.graph.policyBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authorizationPolicy",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "blockMsolPowerShell": "Boolean",
  "enabledPreviewFeatures": [
    "String"
  ],
  "guestUserRoleId": "Guid",
  "permissionGrantPolicyIdsAssignedToDefaultUserRole": [
    "String"
  ]
}
```

