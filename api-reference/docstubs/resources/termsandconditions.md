---
title: "termsAndConditions resource type"
description: "A termsAndConditions entity represents the metadata and contents of a given Terms and Conditions (T&C) policy. T&C policies’ contents are presented to users upon their first attempt to enroll into Intune and subsequently upon edits where an administrator has required re-acceptance. They enable administrators to communicate the provisions to which a user must agree in order to have devices enrolled into Intune."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# termsAndConditions resource type


Namespace: microsoft.graph

A termsAndConditions entity represents the metadata and contents of a given Terms and Conditions (T&C) policy. T&C policies’ contents are presented to users upon their first attempt to enroll into Intune and subsequently upon edits where an administrator has required re-acceptance. They enable administrators to communicate the provisions to which a user must agree in order to have devices enrolled into Intune.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get termsAndConditions](../api/termsandconditions-get.md)|[termsAndConditions](../resources/termsandconditions.md)|Read properties and relationships of a [termsAndConditions](../resources/termsandconditions.md) object.|
|[Update termsAndConditions](../api/termsandconditions-update.md)|[termsAndConditions](../resources/termsandconditions.md)|Update the properties of a [termsAndConditions](../resources/termsandconditions.md) object.|
|[List assignments](../api/termsandconditions-list-assignments.md)|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md) collection|Get the termsAndConditionsAssignments from the assignments navigation property.|
|[Create assignments](../api/termsandconditions-post-assignments.md)|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/termsandconditions-delete-assignments.md)|None|Delete an assignments object.|
|[Update assignments](../api/termsandconditions-update-assignments.md)|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md)|Update the properties of an assignments object.|
|[Get termsAndConditionsAssignment](../api/termsandconditionsassignment-get.md)|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md)|Read properties and relationships of a [termsAndConditionsAssignment](../resources/termsandconditionsassignment.md) object.|
|[List acceptanceStatuses](../api/termsandconditions-list-acceptancestatuses.md)|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) collection|Get the termsAndConditionsAcceptanceStatus from the acceptanceStatuses navigation property.|
|[Create acceptanceStatuses](../api/termsandconditions-post-acceptancestatuses.md)|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md)|Create a new acceptanceStatuses object.|
|[Delete acceptanceStatuses](../api/termsandconditions-delete-acceptancestatuses.md)|None|Delete an acceptanceStatuses object.|
|[Update acceptanceStatuses](../api/termsandconditions-update-acceptancestatuses.md)|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md)|Update the properties of an acceptanceStatuses object.|
|[Get termsAndConditionsAcceptanceStatus](../api/termsandconditionsacceptancestatus-get.md)|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md)|Read properties and relationships of a [termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|acceptanceStatement|String|Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy. This is shown to the user on prompts to accept the T&C policy.|
|bodyText|String|Administrator-supplied body text of the terms and conditions, typically the terms themselves. This is shown to the user on prompts to accept the T&C policy.|
|createdDateTime|DateTimeOffset|DateTime the object was created.|
|description|String|Administrator-supplied description of the T&C policy.|
|displayName|String|Administrator-supplied name for the T&C policy. |
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|title|String|Administrator-supplied title of the terms and conditions. This is shown to the user on prompts to accept the T&C policy.|
|version|Int32|Integer indicating the current version of the terms. Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|acceptanceStatuses|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) collection|The list of acceptance statuses for this T&C policy.|
|assignments|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md) collection|The list of assignments for this T&C policy.|

## JSON representation
Here is a JSON representation of the resource.
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
  "version": 1024
}
```

