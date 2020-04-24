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


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get informationProtection](../api/informationprotection-get.md)|[informationProtection](../resources/informationprotection.md)|Read the properties and relationships of an [informationProtection](../resources/informationprotection.md) object.|
|[Update informationProtection](../api/informationprotection-update.md)|[informationProtection](../resources/informationprotection.md)|Update the properties of an [informationProtection](../resources/informationprotection.md) object.|
|[evaluateLabelsAndPolicies](../api/informationprotection-evaluatelabelsandpolicies.md)|[evaluateLabelsAndPoliciesJobResponse](../resources/evaluatelabelsandpoliciesjobresponse.md)|**TODO: Add Description**|
|[List policy](../api/informationprotection-list-policy.md)|[informationProtectionPolicy](../resources/informationprotectionpolicy.md) collection|Get the informationProtectionPolicies from the policy navigation property.|
|[Create policy](../api/informationprotection-post-policy.md)|[informationProtectionPolicy](../resources/informationprotectionpolicy.md)|Create a new policy object.|
|[Delete policy](../api/informationprotection-delete-policy.md)|None|Delete a [informationProtectionPolicy](../resources/informationprotectionpolicy.md) object.|
|[Update policy](../api/informationprotection-update-policy.md)|[informationProtectionPolicy](../resources/informationprotectionpolicy.md)|Update the properties of a policy object.|
|[Get informationProtectionPolicy](../api/informationprotectionpolicy-get.md)|[informationProtectionPolicy](../resources/informationprotectionpolicy.md)|Read the properties and relationships of an [informationProtectionPolicy](../resources/informationprotectionpolicy.md) object.|
|[List sensitivityLabels](../api/informationprotection-list-sensitivitylabels.md)|[sensitivityLabel](../resources/sensitivitylabel.md) collection|Get the sensitivityLabels from the sensitivityLabels navigation property.|
|[Create sensitivityLabels](../api/informationprotection-post-sensitivitylabels.md)|[sensitivityLabel](../resources/sensitivitylabel.md)|Create a new sensitivityLabels object.|
|[Delete sensitivityLabels](../api/informationprotection-delete-sensitivitylabels.md)|None|Delete a [sensitivityLabel](../resources/sensitivitylabel.md) object.|
|[Update sensitivityLabels](../api/informationprotection-update-sensitivitylabels.md)|[sensitivityLabel](../resources/sensitivitylabel.md)|Update the properties of a sensitivityLabels object.|
|[Get sensitivityLabel](../api/sensitivitylabel-get.md)|[sensitivityLabel](../resources/sensitivitylabel.md)|Read the properties and relationships of a [sensitivityLabel](../resources/sensitivitylabel.md) object.|
|[List sensitivityPolicySettings](../api/informationprotection-list-sensitivitypolicysettings.md)|[sensitivityPolicySettings](../resources/sensitivitypolicysettings.md) collection|Get the sensitivityPolicySettings from the sensitivityPolicySettings navigation property.|
|[Create sensitivityPolicySettings](../api/informationprotection-post-sensitivitypolicysettings.md)|[sensitivityPolicySettings](../resources/sensitivitypolicysettings.md)|Create a new sensitivityPolicySettings object.|
|[Delete sensitivityPolicySettings](../api/informationprotection-delete-sensitivitypolicysettings.md)|None|Delete a [sensitivityPolicySettings](../resources/sensitivitypolicysettings.md) object.|
|[Update sensitivityPolicySettings](../api/informationprotection-update-sensitivitypolicysettings.md)|[sensitivityPolicySettings](../resources/sensitivitypolicysettings.md)|Update the properties of a sensitivityPolicySettings object.|
|[Get sensitivityPolicySettings](../api/sensitivitypolicysettings-get.md)|[sensitivityPolicySettings](../resources/sensitivitypolicysettings.md)|Read the properties and relationships of a [sensitivityPolicySettings](../resources/sensitivitypolicysettings.md) object.|
|[List dataLossPreventionPolicies](../api/informationprotection-list-datalosspreventionpolicies.md)|[dataLossPreventionPolicy](../resources/datalosspreventionpolicy.md) collection|Get the dataLossPreventionPolicies from the dataLossPreventionPolicies navigation property.|
|[Create dataLossPreventionPolicies](../api/informationprotection-post-datalosspreventionpolicies.md)|[dataLossPreventionPolicy](../resources/datalosspreventionpolicy.md)|Create a new dataLossPreventionPolicies object.|
|[Delete dataLossPreventionPolicies](../api/informationprotection-delete-datalosspreventionpolicies.md)|None|Delete a [dataLossPreventionPolicy](../resources/datalosspreventionpolicy.md) object.|
|[Update dataLossPreventionPolicies](../api/informationprotection-update-datalosspreventionpolicies.md)|[dataLossPreventionPolicy](../resources/datalosspreventionpolicy.md)|Update the properties of a dataLossPreventionPolicies object.|
|[Get dataLossPreventionPolicy](../api/datalosspreventionpolicy-get.md)|[dataLossPreventionPolicy](../resources/datalosspreventionpolicy.md)|Read the properties and relationships of a [dataLossPreventionPolicy](../resources/datalosspreventionpolicy.md) object.|
|[List threatAssessmentRequests](../api/informationprotection-list-threatassessmentrequests.md)|[threatAssessmentRequest](../resources/threatassessmentrequest.md) collection|Get the threatAssessmentRequests from the threatAssessmentRequests navigation property.|
|[Create threatAssessmentRequests](../api/informationprotection-post-threatassessmentrequests.md)|[threatAssessmentRequest](../resources/threatassessmentrequest.md)|Create a new threatAssessmentRequests object.|
|[Delete threatAssessmentRequests](../api/informationprotection-delete-threatassessmentrequests.md)|None|Delete a [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.|
|[Update threatAssessmentRequests](../api/informationprotection-update-threatassessmentrequests.md)|[threatAssessmentRequest](../resources/threatassessmentrequest.md)|Update the properties of a threatAssessmentRequests object.|
|[Get threatAssessmentRequest](../api/threatassessmentrequest-get.md)|[threatAssessmentRequest](../resources/threatassessmentrequest.md)|Read the properties and relationships of a [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|dataLossPreventionPolicies|[dataLossPreventionPolicy](../resources/datalosspreventionpolicy.md) collection|**TODO: Add Description**|
|policy|[informationProtectionPolicy](../resources/informationprotectionpolicy.md)|**TODO: Add Description**|
|sensitivityLabels|[sensitivityLabel](../resources/sensitivitylabel.md) collection|**TODO: Add Description**|
|sensitivityPolicySettings|[sensitivityPolicySettings](../resources/sensitivitypolicysettings.md)|**TODO: Add Description**|
|threatAssessmentRequests|[threatAssessmentRequest](../resources/threatassessmentrequest.md) collection|**TODO: Add Description**|

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

