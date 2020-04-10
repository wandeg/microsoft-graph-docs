---
title: "policySet resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# policySet resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get policySet](../api/policyset-get.md)|[policySet](../resources/policyset.md)|Read properties and relationships of the [policySet](../resources/policyset.md) object.|
|[Update policySet](../api/policyset-update.md)|[policySet](../resources/policyset.md)|Update the properties of a [policySet](../resources/policyset.md) object.|
|[update](../api/policyset-update.md)|None||
|[getPolicySets](../api/policyset-getpolicysets.md)|[policySet](../resources/policyset.md) collection||
|[List assignments](../api/policyset-list-assignments.md)|[policySetAssignment](../resources/policysetassignment.md) collection|Get the policySetAssignments from the assignments navigation property.|
|[Add assignments](../api/policyset-post-assignments.md)|[policySetAssignment](../resources/policysetassignment.md)|Add assignments by posting to the assignments collection.|
|[List items](../api/policyset-list-items.md)|[policySetItem](../resources/policysetitem.md) collection|Get the policySetItems from the items navigation property.|
|[Add items](../api/policyset-post-items.md)|[policySetItem](../resources/policysetitem.md)|Add items by posting to the items collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset||
|description|String||
|displayName|String||
|errorCode|Enumeration| Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|String collection||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|roleScopeTags|String collection||
|status|Enumeration| Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[policySetAssignment](../resources/policysetassignment.md) collection||
|items|[policySetItem](../resources/policysetitem.md) collection||

## JSON representation
Here is a JSON representation of the resource.
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

