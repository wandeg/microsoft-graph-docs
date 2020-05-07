---
title: "deviceEnrollmentConfiguration resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceEnrollmentConfiguration resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[hasPayloadLinks](../api/deviceenrollmentconfiguration-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/haspayloadlinkresultitem.md) collection|**TODO: Add Description**|
|[setPriority](../api/deviceenrollmentconfiguration-setpriority.md)|None|**TODO: Add Description**|
|[assign](../api/deviceenrollmentconfiguration-assign.md)|None|**TODO: Add Description**|
|[List assignments](../api/deviceenrollmentconfiguration-list-assignments.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) collection|Get the enrollmentConfigurationAssignments from the assignments navigation property.|
|[Create assignments](../api/deviceenrollmentconfiguration-post-assignments.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/deviceenrollmentconfiguration-delete-assignments.md)|None|Delete an [enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) object.|
|[Update assignments](../api/deviceenrollmentconfiguration-update-assignments.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md)|Update the properties of an assignments object.|
|[Get enrollmentConfigurationAssignment](../api/enrollmentconfigurationassignment-get.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md)|Read the properties and relationships of an [enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|priority|Int32|**TODO: Add Description**|
|version|Int32|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentConfiguration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": "Integer",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": "Integer"
}
```

