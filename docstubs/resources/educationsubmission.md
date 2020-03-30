---
title: "educationSubmission resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationSubmission resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationSubmission](../api/educationsubmission-get.md)|[educationSubmission](../resources/educationsubmission.md)|Read properties and relationships of the [educationSubmission](../resources/educationsubmission.md) object.|
|[Update educationSubmission](../api/educationsubmission-update.md)|[educationSubmission](../resources/educationsubmission.md)|Update the properties of a [educationSubmission](../resources/educationsubmission.md) object.|
|[return](../api/educationsubmission-return.md)|[educationSubmission](../resources/educationsubmission.md)||
|[submit](../api/educationsubmission-submit.md)|[educationSubmission](../resources/educationsubmission.md)||
|[unsubmit](../api/educationsubmission-unsubmit.md)|[educationSubmission](../resources/educationsubmission.md)||
|[List resources](../api/educationsubmission-list-resources.md)|[educationSubmissionResource](../resources/educationsubmissionresource.md) collection|Get the educationSubmissionResources from the resources navigation property.|
|[Add resources](../api/educationsubmission-post-resources.md)|[educationSubmissionResource](../resources/educationsubmissionresource.md)|Add resources by posting to the resources collection.|
|[List submittedResources](../api/educationsubmission-list-submittedresources.md)|[educationSubmissionResource](../resources/educationsubmissionresource.md) collection|Get the educationSubmissionResources from the submittedResources navigation property.|
|[Add submittedResources](../api/educationsubmission-post-submittedresources.md)|[educationSubmissionResource](../resources/educationsubmissionresource.md)|Add submittedResources by posting to the submittedResources collection.|
|[List outcomes](../api/educationsubmission-list-outcomes.md)|[educationOutcome](../resources/educationoutcome.md) collection|Get the educationOutcomes from the outcomes navigation property.|
|[Add outcomes](../api/educationsubmission-post-outcomes.md)|[educationOutcome](../resources/educationoutcome.md)|Add outcomes by posting to the outcomes collection.|
|[List submissions](../api/educationassignment-list-submissions.md)|[educationSubmission](../resources/educationsubmission.md) collection|Get the educationSubmissions from the submissions navigation property.|
|[Add submissions](../api/educationassignment-post-submissions.md)|[educationSubmission](../resources/educationsubmission.md)|Add submissions by posting to the submissions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|recipient|[educationSubmissionRecipient](../resources/educationsubmissionrecipient.md)||
|releasedBy|[identitySet](../resources/identityset.md)||
|releasedDateTime|DateTimeOffset||
|resourcesFolderUrl|String||
|returnedBy|[identitySet](../resources/identityset.md)||
|returnedDateTime|DateTimeOffset||
|status|Enumeration| Possible values are: `working`, `submitted`, `released`, `returned`, `unknownFutureValue`.|
|submittedBy|[identitySet](../resources/identityset.md)||
|submittedDateTime|DateTimeOffset||
|unsubmittedBy|[identitySet](../resources/identityset.md)||
|unsubmittedDateTime|DateTimeOffset||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|outcomes|[educationOutcome](../resources/educationoutcome.md) collection||
|resources|[educationSubmissionResource](../resources/educationsubmissionresource.md) collection||
|submittedResources|[educationSubmissionResource](../resources/educationsubmissionresource.md) collection||

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

