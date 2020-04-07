---
title: "informationProtection resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# informationProtection resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get informationProtection](../api/informationprotection-get.md)|[informationProtection](../resources/informationprotection.md)|Read properties and relationships of the [informationProtection](../resources/informationprotection.md) object.|
|[Update informationProtection](../api/informationprotection-update.md)|[informationProtection](../resources/informationprotection.md)|Update the properties of a [informationProtection](../resources/informationprotection.md) object.|
|[evaluateLabelsAndPolicies](../api/informationprotection-evaluatelabelsandpolicies.md)|[evaluateLabelsAndPoliciesJobResponse](../resources/evaluatelabelsandpoliciesjobresponse.md)||
|[Get informationProtectionPolicy](../api/informationprotectionpolicy-get.md)|[informationProtectionPolicy](../resources/informationprotectionpolicy.md)|Read properties and relationships of the [informationProtectionPolicy](../resources/informationprotectionpolicy.md) object.|
|[List sensitivityLabels](../api/informationprotection-list-sensitivitylabels.md)|[sensitivityLabel](../resources/sensitivitylabel.md) collection|Get the sensitivityLabels from the sensitivityLabels navigation property.|
|[Add sensitivityLabels](../api/informationprotection-post-sensitivitylabels.md)|[sensitivityLabel](../resources/sensitivitylabel.md)|Add sensitivityLabels by posting to the sensitivityLabels collection.|
|[Get sensitivityPolicySettings](../api/sensitivitypolicysettings-get.md)|[sensitivityPolicySettings](../resources/sensitivitypolicysettings.md)|Read properties and relationships of the [sensitivityPolicySettings](../resources/sensitivitypolicysettings.md) object.|
|[List dataLossPreventionPolicies](../api/informationprotection-list-datalosspreventionpolicies.md)|[dataLossPreventionPolicy](../resources/datalosspreventionpolicy.md) collection|Get the dataLossPreventionPolicies from the dataLossPreventionPolicies navigation property.|
|[Add dataLossPreventionPolicies](../api/informationprotection-post-datalosspreventionpolicies.md)|[dataLossPreventionPolicy](../resources/datalosspreventionpolicy.md)|Add dataLossPreventionPolicies by posting to the dataLossPreventionPolicies collection.|
|[List threatAssessmentRequests](../api/informationprotection-list-threatassessmentrequests.md)|[threatAssessmentRequest](../resources/threatassessmentrequest.md) collection|Get the threatAssessmentRequests from the threatAssessmentRequests navigation property.|
|[Add threatAssessmentRequests](../api/informationprotection-post-threatassessmentrequests.md)|[threatAssessmentRequest](../resources/threatassessmentrequest.md)|Add threatAssessmentRequests by posting to the threatAssessmentRequests collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|dataLossPreventionPolicies|[dataLossPreventionPolicy](../resources/datalosspreventionpolicy.md) collection||
|policy|[informationProtectionPolicy](../resources/informationprotectionpolicy.md)||
|sensitivityLabels|[sensitivityLabel](../resources/sensitivitylabel.md) collection||
|sensitivityPolicySettings|[sensitivityPolicySettings](../resources/sensitivitypolicysettings.md)||
|threatAssessmentRequests|[threatAssessmentRequest](../resources/threatassessmentrequest.md) collection||

## JSON representation
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

