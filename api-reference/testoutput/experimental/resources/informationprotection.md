---
title: "informationProtection resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# informationProtection resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List informationProtections](../api/informationprotection-list.md)|[informationProtection](../resources/informationProtection.md) collection|List properties and relationships of the [informationProtection](../resources/informationprotection.md) objects.|
|[Get informationProtection](../api/informationprotection-get.md)|[informationProtection](../resources/informationProtection.md)|Read properties and relationships of the [informationProtection](../resources/informationprotection.md) object.|
|[Create informationProtection](../api/informationprotection-create.md)|[informationProtection](../resources/informationProtection.md)|Create a new [informationProtection](../resources/informationprotection.md) object.|
|[Delete informationProtection](../api/informationprotection-delete.md)|None|Deletes a [informationProtection](../resources/informationprotection.md).|
|[Update informationProtection](../api/informationprotection-update.md)|[informationProtection](../resources/informationProtection.md)|Update the properties of a [informationProtection](../resources/informationprotection.md) object.|
|[evaluateLabelsAndPolicies](../api/informationprotection-evaluatelabelsandpolicies.md)|[evaluateLabelsAndPoliciesJobResponse](../resources/evaluateLabelsAndPoliciesJobResponse.md)||
|[Get informationProtectionPolicy](../api/informationprotectionpolicy-get.md)|[informationProtectionPolicy](../resources/informationProtectionPolicy.md)|Read properties and relationships of the [informationProtectionPolicy](../resources/informationprotectionpolicy.md) object.|
|[List sensitivityLabels](../api/informationprotection-list-sensitivitylabels.md)|[sensitivityLabel](../resources/sensitivityLabel.md) collection|Get the sensitivityLabels from the sensitivityLabels navigation property.|
|[Add sensitivityLabels](../api/informationprotection-post-sensitivitylabels.md)|[sensitivityLabel](../resources/sensitivityLabel.md)|Add sensitivityLabels by posting to the sensitivityLabels collection.|
|[Get sensitivityPolicySettings](../api/sensitivitypolicysettings-get.md)|[sensitivityPolicySettings](../resources/sensitivityPolicySettings.md)|Read properties and relationships of the [sensitivityPolicySettings](../resources/sensitivitypolicysettings.md) object.|
|[List dataLossPreventionPolicies](../api/informationprotection-list-datalosspreventionpolicies.md)|[dataLossPreventionPolicy](../resources/dataLossPreventionPolicy.md) collection|Get the dataLossPreventionPolicies from the dataLossPreventionPolicies navigation property.|
|[Add dataLossPreventionPolicies](../api/informationprotection-post-datalosspreventionpolicies.md)|[dataLossPreventionPolicy](../resources/dataLossPreventionPolicy.md)|Add dataLossPreventionPolicies by posting to the dataLossPreventionPolicies collection.|
|[List threatAssessmentRequests](../api/informationprotection-list-threatassessmentrequests.md)|[threatAssessmentRequest](../resources/threatAssessmentRequest.md) collection|Get the threatAssessmentRequests from the threatAssessmentRequests navigation property.|
|[Add threatAssessmentRequests](../api/informationprotection-post-threatassessmentrequests.md)|[threatAssessmentRequest](../resources/threatAssessmentRequest.md)|Add threatAssessmentRequests by posting to the threatAssessmentRequests collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|dataLossPreventionPolicies|[dataLossPreventionPolicy](../resources/dataLossPreventionPolicy.md) collection||
|policy|[informationProtectionPolicy](../resources/informationProtectionPolicy.md)||
|sensitivityLabels|[sensitivityLabel](../resources/sensitivityLabel.md) collection||
|sensitivityPolicySettings|[sensitivityPolicySettings](../resources/sensitivityPolicySettings.md)||
|threatAssessmentRequests|[threatAssessmentRequest](../resources/threatAssessmentRequest.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
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

