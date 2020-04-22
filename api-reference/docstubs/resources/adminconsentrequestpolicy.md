---
title: "adminConsentRequestPolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# adminConsentRequestPolicy resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get adminConsentRequestPolicy](../api/adminconsentrequestpolicy-get.md)|[adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md)|Read properties and relationships of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.|
|[Update adminConsentRequestPolicy](../api/adminconsentrequestpolicy-update.md)|[adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md)|Update the properties of a [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isEnabled|Boolean|**TODO: Add Description**|
|notifyReviewers|Boolean|**TODO: Add Description**|
|remindersEnabled|Boolean|**TODO: Add Description**|
|requestDurationInDays|Int32|**TODO: Add Description**|
|reviewers|[accessReviewScope](../resources/accessreviewscope.md) collection|**TODO: Add Description**|
|version|Int32|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.adminConsentRequestPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsentRequestPolicy",
  "id": "String (identifier)",
  "isEnabled": true,
  "version": 1024,
  "notifyReviewers": true,
  "remindersEnabled": true,
  "requestDurationInDays": 1024,
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ]
}
```

