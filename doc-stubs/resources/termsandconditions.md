---
title: "termsAndConditions resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# termsAndConditions resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List groupAssignments](../api/termsandconditions-list-groupassignments.md)|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) collection|Get the termsAndConditionsGroupAssignments from the groupAssignments navigation property.|
|[Create groupAssignments](../api/termsandconditions-post-groupassignments.md)|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md)|Create a new groupAssignments object.|
|[Delete groupAssignments](../api/termsandconditions-delete-groupassignments.md)|None|Delete a [termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) object.|
|[Update groupAssignments](../api/termsandconditions-update-groupassignments.md)|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md)|Update the properties of a groupAssignments object.|
|[Get termsAndConditionsGroupAssignment](../api/termsandconditionsgroupassignment-get.md)|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md)|Read the properties and relationships of a [termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) object.|
|[List assignments](../api/termsandconditions-list-assignments.md)|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md) collection|Get the termsAndConditionsAssignments from the assignments navigation property.|
|[Create assignments](../api/termsandconditions-post-assignments.md)|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/termsandconditions-delete-assignments.md)|None|Delete an [termsAndConditionsAssignment](../resources/termsandconditionsassignment.md) object.|
|[Update assignments](../api/termsandconditions-update-assignments.md)|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md)|Update the properties of an assignments object.|
|[Get termsAndConditionsAssignment](../api/termsandconditionsassignment-get.md)|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md)|Read the properties and relationships of a [termsAndConditionsAssignment](../resources/termsandconditionsassignment.md) object.|
|[List acceptanceStatuses](../api/termsandconditions-list-acceptancestatuses.md)|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) collection|Get the termsAndConditionsAcceptanceStatus from the acceptanceStatuses navigation property.|
|[Create acceptanceStatuses](../api/termsandconditions-post-acceptancestatuses.md)|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md)|Create a new acceptanceStatuses object.|
|[Delete acceptanceStatuses](../api/termsandconditions-delete-acceptancestatuses.md)|None|Delete an [termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) object.|
|[Update acceptanceStatuses](../api/termsandconditions-update-acceptancestatuses.md)|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md)|Update the properties of an acceptanceStatuses object.|
|[Get termsAndConditionsAcceptanceStatus](../api/termsandconditionsacceptancestatus-get.md)|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md)|Read the properties and relationships of a [termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|acceptanceStatement|String|**TODO: Add Description**|
|bodyText|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|
|title|String|**TODO: Add Description**|
|version|Int32|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|acceptanceStatuses|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) collection|**TODO: Add Description**|
|assignments|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md) collection|**TODO: Add Description**|
|groupAssignments|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditions",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "title": "String",
  "bodyText": "String",
  "acceptanceStatement": "String",
  "version": "Integer",
  "roleScopeTagIds": [
    "String"
  ]
}
```

