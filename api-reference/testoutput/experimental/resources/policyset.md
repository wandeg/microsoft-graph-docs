---
title: "policySet resource type"
description: "A class containing the properties used for PolicySet."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# policySet resource type


Namespace: microsoft.graph

A class containing the properties used for PolicySet.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List policySets](../api/policyset-list.md)|[policySet](../resources/policyset.md) collection|List properties and relationships of the [policySet](../resources/policyset.md) objects.|
|[Get policySet](../api/policyset-get.md)|[policySet](../resources/policyset.md)|Read properties and relationships of the [policySet](../resources/policyset.md) object.|
|[Create policySet](../api/policyset-create.md)|[policySet](../resources/policyset.md)|Create a new [policySet](../resources/policyset.md) object.|
|[Delete policySet](../api/policyset-delete.md)|None|Deletes a [policySet](../resources/policyset.md).|
|[Update policySet](../api/policyset-update.md)|[policySet](../resources/policyset.md)|Update the properties of a [policySet](../resources/policyset.md) object.|
|[update](../api/policyset-update.md)|None||
|[getPolicySets](../api/policyset-getpolicysets.md)|[policySet](../resources/policyset.md) collection||
|[List assignments](../api/policyset-list-assignments.md)|[policySetAssignment](../resources/policysetassignment.md) collection|Get the policySetAssignments from the assignments navigation property.|
|[Add assignments](../api/policyset-post-assignments.md)|[policySetAssignment](../resources/policysetassignment.md)|Add assignments by posting to the assignments collection.|
|[List items](../api/policyset-list-items.md)|[policySetItem](../resources/policysetitem.md) collection|Get the policySetItems from the items navigation property.|
|[Add items](../api/policyset-post-items.md)|[policySetItem](../resources/policysetitem.md)|Add items by posting to the items collection.|
|[List policySets](../api/intune-apps-deviceappmanagement-list-policysets.md)|[policySet](../resources/policyset.md) collection|Get the policySets from the policySets navigation property.|
|[Add policySets](../api/intune-apps-deviceappmanagement-post-policysets.md)|[policySet](../resources/policyset.md)|Add policySets by posting to the policySets collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Creation time of the PolicySet.|
|description|String|Description of the PolicySet.|
|displayName|String|DisplayName of the PolicySet.|
|errorCode|Enumeration|Error code if any occured. Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|String collection|Tags of the guided deployment|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Last modified time of the PolicySet.|
|roleScopeTags|String collection|RoleScopeTags of the PolicySet|
|status|Enumeration|Validation/assignment status of the PolicySet. Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[policySetAssignment](../resources/policysetassignment.md) collection|Assignments of the PolicySet.|
|items|[policySetItem](../resources/policysetitem.md) collection|Items of the PolicySet with maximum count 100.|

## JSON Representation
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

