---
title: "enrollmentConfigurationAssignment resource type"
description: "Enrollment Configuration Assignment"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# enrollmentConfigurationAssignment resource type


Namespace: microsoft.graph

Enrollment Configuration Assignment


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List enrollmentConfigurationAssignments](../api/enrollmentconfigurationassignment-list.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) collection|List properties and relationships of the [enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) objects.|
|[Get enrollmentConfigurationAssignment](../api/enrollmentconfigurationassignment-get.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md)|Read properties and relationships of the [enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) object.|
|[Create enrollmentConfigurationAssignment](../api/enrollmentconfigurationassignment-create.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md)|Create a new [enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) object.|
|[Delete enrollmentConfigurationAssignment](../api/enrollmentconfigurationassignment-delete.md)|None|Deletes a [enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md).|
|[Update enrollmentConfigurationAssignment](../api/enrollmentconfigurationassignment-update.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md)|Update the properties of a [enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|source|Enumeration|Type of resource used for deployment to a group, direct or policySet. Possible values are: `direct`, `policySets`.|
|sourceId|String|Identifier for resource used for deployment to a group|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-apps-deviceandappmanagementassignmenttarget.md)|Represents an assignment to managed devices in the tenant|

## Relationships
None

## JSON Representation
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

