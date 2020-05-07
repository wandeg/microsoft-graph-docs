---
title: "policySet resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# policySet resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[update](../api/policyset-update.md)|None|**TODO: Add Description**|
|[getPolicySets](../api/policyset-getpolicysets.md)|[policySet](../resources/policyset.md) collection|**TODO: Add Description**|
|[List assignments](../api/policyset-list-assignments.md)|[policySetAssignment](../resources/policysetassignment.md) collection|Get the policySetAssignments from the assignments navigation property.|
|[Create assignments](../api/policyset-post-assignments.md)|[policySetAssignment](../resources/policysetassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/policyset-delete-assignments.md)|None|Delete an [policySetAssignment](../resources/policysetassignment.md) object.|
|[Update assignments](../api/policyset-update-assignments.md)|[policySetAssignment](../resources/policysetassignment.md)|Update the properties of an assignments object.|
|[Get policySetAssignment](../api/policysetassignment-get.md)|[policySetAssignment](../resources/policysetassignment.md)|Read the properties and relationships of a [policySetAssignment](../resources/policysetassignment.md) object.|
|[List items](../api/policyset-list-items.md)|[policySetItem](../resources/policysetitem.md) collection|Get the policySetItems from the items navigation property.|
|[Create items](../api/policyset-post-items.md)|[policySetItem](../resources/policysetitem.md)|Create a new items object.|
|[Delete items](../api/policyset-delete-items.md)|None|Delete an [policySetItem](../resources/policysetitem.md) object.|
|[Update items](../api/policyset-update-items.md)|[policySetItem](../resources/policysetitem.md)|Update the properties of an items object.|
|[Get policySetItem](../api/policysetitem-get.md)|[policySetItem](../resources/policysetitem.md)|Read the properties and relationships of a [policySetItem](../resources/policysetitem.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|errorCode|errorCode|**TODO: Add Description**. Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|String collection|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|roleScopeTags|String collection|**TODO: Add Description**|
|status|policySetStatus|**TODO: Add Description**. Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[policySetAssignment](../resources/policysetassignment.md) collection|**TODO: Add Description**|
|items|[policySetItem](../resources/policysetitem.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policySet",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policySet",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ],
  "roleScopeTags": [
    "String"
  ]
}
```

