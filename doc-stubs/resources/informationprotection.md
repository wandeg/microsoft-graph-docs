---
title: "informationProtection resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# informationProtection resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List threatAssessmentRequests](../api/informationprotection-list-threatassessmentrequests.md)|[threatAssessmentRequest](../resources/threatassessmentrequest.md) collection|Get the threatAssessmentRequests from the threatAssessmentRequests navigation property.|
|[Create threatAssessmentRequests](../api/informationprotection-post-threatassessmentrequests.md)|[threatAssessmentRequest](../resources/threatassessmentrequest.md)|Create a new threatAssessmentRequests object.|
|[Delete threatAssessmentRequests](../api/informationprotection-delete-threatassessmentrequests.md)|None|Delete a [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.|
|[Update threatAssessmentRequests](../api/informationprotection-update-threatassessmentrequests.md)|[threatAssessmentRequest](../resources/threatassessmentrequest.md)|Update the properties of a threatAssessmentRequests object.|
|[Get threatAssessmentRequests](../api/informationprotection-get-threatassessmentrequest.md)|[threatAssessmentRequest](../resources/threatassessmentrequest.md)|Read the properties and relationships of a [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|threatAssessmentRequests|[threatAssessmentRequest](../resources/threatassessmentrequest.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.informationProtection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.informationProtection",
  "id": "String (identifier)"
}
```

