---
title: "enrollmentConfigurationAssignment resource type"
description: "Enrollment Configuration Assignment"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# enrollmentConfigurationAssignment resource type


Namespace: microsoft.graph

Enrollment Configuration Assignment


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get enrollmentConfigurationAssignment](../api/enrollmentconfigurationassignment-get.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md)|Read the properties and relationships of an [enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) object.|
|[Update enrollmentConfigurationAssignment](../api/enrollmentconfigurationassignment-update.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md)|Update the properties of an [enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|source|deviceAndAppManagementAssignmentSource|Type of resource used for deployment to a group, direct or policySet. Possible values are: `direct`, `policySets`.|
|sourceId|String|Identifier for resource used for deployment to a group|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)|Represents an assignment to managed devices in the tenant|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentConfigurationAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "String",
  "sourceId": "String"
}
```

