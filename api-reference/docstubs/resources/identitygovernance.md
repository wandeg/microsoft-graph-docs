---
title: "identityGovernance resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# identityGovernance resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get identityGovernance](../api/identitygovernance-get.md)|[identityGovernance](../resources/identitygovernance.md)|Read the properties and relationships of an [identityGovernance](../resources/identitygovernance.md) object.|
|[Update identityGovernance](../api/identitygovernance-update.md)|[identityGovernance](../resources/identitygovernance.md)|Update the properties of an [identityGovernance](../resources/identitygovernance.md) object.|
|[List entitlementManagement](../api/identitygovernance-list-entitlementmanagement.md)|[entitlementManagement](../resources/entitlementmanagement.md) collection|Get the entitlementManagements from the entitlementManagement navigation property.|
|[Create entitlementManagement](../api/identitygovernance-post-entitlementmanagement.md)|[entitlementManagement](../resources/entitlementmanagement.md)|Create a new entitlementManagement object.|
|[Delete entitlementManagement](../api/identitygovernance-delete-entitlementmanagement.md)|None|Delete an [entitlementManagement](../resources/entitlementmanagement.md) object.|
|[Update entitlementManagement](../api/identitygovernance-update-entitlementmanagement.md)|[entitlementManagement](../resources/entitlementmanagement.md)|Update the properties of an entitlementManagement object.|
|[Get entitlementManagement](../api/entitlementmanagement-get.md)|[entitlementManagement](../resources/entitlementmanagement.md)|Read the properties and relationships of an [entitlementManagement](../resources/entitlementmanagement.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|entitlementManagement|[entitlementManagement](../resources/entitlementmanagement.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityGovernance",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.identityGovernance",
  "id": "String (identifier)"
}
```

