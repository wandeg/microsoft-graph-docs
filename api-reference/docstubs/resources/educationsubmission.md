---
title: "educationSubmission resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# educationSubmission resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationSubmission](../api/educationsubmission-get.md)|[educationSubmission](../resources/educationsubmission.md)|Read the properties and relationships of an [educationSubmission](../resources/educationsubmission.md) object.|
|[Update educationSubmission](../api/educationsubmission-update.md)|[educationSubmission](../resources/educationsubmission.md)|Update the properties of an [educationSubmission](../resources/educationsubmission.md) object.|
|[return](../api/educationsubmission-return.md)|[educationSubmission](../resources/educationsubmission.md)|**TODO: Add Description**|
|[submit](../api/educationsubmission-submit.md)|[educationSubmission](../resources/educationsubmission.md)|**TODO: Add Description**|
|[unsubmit](../api/educationsubmission-unsubmit.md)|[educationSubmission](../resources/educationsubmission.md)|**TODO: Add Description**|
|[List resources](../api/educationsubmission-list-resources.md)|[educationSubmissionResource](../resources/educationsubmissionresource.md) collection|Get the educationSubmissionResources from the resources navigation property.|
|[Create resources](../api/educationsubmission-post-resources.md)|[educationSubmissionResource](../resources/educationsubmissionresource.md)|Create a new resources object.|
|[Delete resources](../api/educationsubmission-delete-resources.md)|None|Delete a [educationSubmissionResource](../resources/educationsubmissionresource.md) object.|
|[Update resources](../api/educationsubmission-update-resources.md)|[educationSubmissionResource](../resources/educationsubmissionresource.md)|Update the properties of a resources object.|
|[Get educationSubmissionResource](../api/educationsubmissionresource-get.md)|[educationSubmissionResource](../resources/educationsubmissionresource.md)|Read the properties and relationships of an [educationSubmissionResource](../resources/educationsubmissionresource.md) object.|
|[List submittedResources](../api/educationsubmission-list-submittedresources.md)|[educationSubmissionResource](../resources/educationsubmissionresource.md) collection|Get the educationSubmissionResources from the submittedResources navigation property.|
|[Create submittedResources](../api/educationsubmission-post-submittedresources.md)|[educationSubmissionResource](../resources/educationsubmissionresource.md)|Create a new submittedResources object.|
|[Delete submittedResources](../api/educationsubmission-delete-submittedresources.md)|None|Delete a [educationSubmissionResource](../resources/educationsubmissionresource.md) object.|
|[Update submittedResources](../api/educationsubmission-update-submittedresources.md)|[educationSubmissionResource](../resources/educationsubmissionresource.md)|Update the properties of a submittedResources object.|
|[Get educationSubmissionResource](../api/educationsubmissionresource-get.md)|[educationSubmissionResource](../resources/educationsubmissionresource.md)|Read the properties and relationships of an [educationSubmissionResource](../resources/educationsubmissionresource.md) object.|
|[List outcomes](../api/educationsubmission-list-outcomes.md)|[educationOutcome](../resources/educationoutcome.md) collection|Get the educationOutcomes from the outcomes navigation property.|
|[Create outcomes](../api/educationsubmission-post-outcomes.md)|[educationOutcome](../resources/educationoutcome.md)|Create a new outcomes object.|
|[Delete outcomes](../api/educationsubmission-delete-outcomes.md)|None|Delete an [educationOutcome](../resources/educationoutcome.md) object.|
|[Update outcomes](../api/educationsubmission-update-outcomes.md)|[educationOutcome](../resources/educationoutcome.md)|Update the properties of an outcomes object.|
|[Get educationOutcome](../api/educationoutcome-get.md)|[educationOutcome](../resources/educationoutcome.md)|Read the properties and relationships of an [educationOutcome](../resources/educationoutcome.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|recipient|[educationSubmissionRecipient](../resources/educationsubmissionrecipient.md)|**TODO: Add Description**|
|releasedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|releasedDateTime|DateTimeOffset|**TODO: Add Description**|
|resourcesFolderUrl|String|**TODO: Add Description**|
|returnedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|returnedDateTime|DateTimeOffset|**TODO: Add Description**|
|status|educationSubmissionStatus|**TODO: Add Description**. Possible values are: `working`, `submitted`, `released`, `returned`, `unknownFutureValue`.|
|submittedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|submittedDateTime|DateTimeOffset|**TODO: Add Description**|
|unsubmittedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|unsubmittedDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|outcomes|[educationOutcome](../resources/educationoutcome.md) collection|**TODO: Add Description**|
|resources|[educationSubmissionResource](../resources/educationsubmissionresource.md) collection|**TODO: Add Description**|
|submittedResources|[educationSubmissionResource](../resources/educationsubmissionresource.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationSubmission",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationSubmission",
  "id": "String (identifier)",
  "recipient": {
    "@odata.type": "microsoft.graph.educationSubmissionRecipient"
  },
  "status": "String",
  "submittedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "submittedDateTime": "String (timestamp)",
  "unsubmittedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "unsubmittedDateTime": "String (timestamp)",
  "releasedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "releasedDateTime": "String (timestamp)",
  "returnedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "returnedDateTime": "String (timestamp)",
  "resourcesFolderUrl": "String"
}
```

