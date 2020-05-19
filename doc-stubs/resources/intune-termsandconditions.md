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
|[List assignments](../api/intune-termsandconditions-list-assignments.md)|[termsAndConditionsAssignment](../resources/intune-termsandconditionsassignment.md) collection|Get the termsAndConditionsAssignments from the assignments navigation property.|
|[Create assignments](../api/intune-termsandconditions-post-assignments.md)|[termsAndConditionsAssignment](../resources/intune-termsandconditionsassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/intune-termsandconditions-delete-assignments.md)|None|Delete a [termsAndConditionsAssignment](../resources/intune-termsandconditionsassignment.md) object.|
|[Update assignments](../api/intune-termsandconditions-update-assignments.md)|[termsAndConditionsAssignment](../resources/intune-termsandconditionsassignment.md)|Update the properties of an assignments object.|
|[Get assignments](../api/intune-termsandconditions-get-termsandconditionsassignment.md)|[termsAndConditionsAssignment](../resources/intune-termsandconditionsassignment.md)|Read the properties and relationships of a [termsAndConditionsAssignment](../resources/intune-termsandconditionsassignment.md) object.|
|[List acceptanceStatuses](../api/intune-termsandconditions-list-acceptancestatuses.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-termsandconditionsacceptancestatus.md) collection|Get the termsAndConditionsAcceptanceStatus from the acceptanceStatuses navigation property.|
|[Create acceptanceStatuses](../api/intune-termsandconditions-post-acceptancestatuses.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-termsandconditionsacceptancestatus.md)|Create a new acceptanceStatuses object.|
|[Delete acceptanceStatuses](../api/intune-termsandconditions-delete-acceptancestatuses.md)|None|Delete a [termsAndConditionsAcceptanceStatus](../resources/intune-termsandconditionsacceptancestatus.md) object.|
|[Update acceptanceStatuses](../api/intune-termsandconditions-update-acceptancestatuses.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-termsandconditionsacceptancestatus.md)|Update the properties of an acceptanceStatuses object.|
|[Get acceptanceStatuses](../api/intune-termsandconditions-get-termsandconditionsacceptancestatus.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-termsandconditionsacceptancestatus.md)|Read the properties and relationships of a [termsAndConditionsAcceptanceStatus](../resources/intune-termsandconditionsacceptancestatus.md) object.|

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
|title|String|**TODO: Add Description**|
|version|Int32|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|acceptanceStatuses|[termsAndConditionsAcceptanceStatus](../resources/intune-termsandconditionsacceptancestatus.md) collection|**TODO: Add Description**|
|assignments|[termsAndConditionsAssignment](../resources/intune-termsandconditionsassignment.md) collection|**TODO: Add Description**|

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
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "title": "String",
  "bodyText": "String",
  "acceptanceStatement": "String",
  "version": "Integer"
}
```

