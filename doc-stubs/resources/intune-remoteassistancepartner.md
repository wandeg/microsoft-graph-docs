---
title: "remoteAssistancePartner resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# remoteAssistancePartner resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List remoteAssistancePartners](../api/intune-devicemanagement-list-remoteassistancepartners.md)|[remoteAssistancePartner](../resources/intune-remoteassistancepartner.md) collection|Get the remoteAssistancePartners from the remoteAssistancePartners navigation property.|
|[Create remoteAssistancePartners](../api/intune-devicemanagement-post-remoteassistancepartners.md)|[remoteAssistancePartner](../resources/intune-remoteassistancepartner.md)|Create a new remoteAssistancePartners object.|
|[Delete remoteAssistancePartners](../api/intune-devicemanagement-delete-remoteassistancepartners.md)|None|Delete a [remoteAssistancePartner](../resources/intune-remoteassistancepartner.md) object.|
|[Update remoteAssistancePartners](../api/intune-devicemanagement-update-remoteassistancepartners.md)|[remoteAssistancePartner](../resources/intune-remoteassistancepartner.md)|Update the properties of a remoteAssistancePartners object.|
|[Get remoteAssistancePartners](../api/intune-devicemanagement-get-remoteassistancepartner.md)|[remoteAssistancePartner](../resources/intune-remoteassistancepartner.md)|Read the properties and relationships of a [remoteAssistancePartner](../resources/intune-remoteassistancepartner.md) object.|
|[beginOnboarding](../api/intune-remoteassistancepartner-beginonboarding.md)|None|**TODO: Add Description**|
|[disconnect](../api/intune-remoteassistancepartner-disconnect.md)|None|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastConnectionDateTime|DateTimeOffset|**TODO: Add Description**|
|onboardingStatus|remoteAssistanceOnboardingStatus|**TODO: Add Description**. Possible values are: `notOnboarded`, `onboarding`, `onboarded`.|
|onboardingUrl|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteAssistancePartner",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "String (identifier)",
  "displayName": "String",
  "onboardingUrl": "String",
  "onboardingStatus": "String",
  "lastConnectionDateTime": "String (timestamp)"
}
```

