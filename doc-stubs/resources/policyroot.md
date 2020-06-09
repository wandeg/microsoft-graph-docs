---
title: "policyRoot resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# policyRoot resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List policyRoots](../api/policyroot-list.md)|[policyRoot](../resources/policyroot.md) collection|Get a list of the [policyRoot](../resources/policyroot.md) objects and their properties.|
|[Create policyRoot](../api/policyroot-create.md)|[policyRoot](../resources/policyroot.md)|Create a new [policyRoot](../resources/policyroot.md) object.|
|[Get policyRoot](../api/policyroot-get.md)|[policyRoot](../resources/policyroot.md)|Read the properties and relationships of a [policyRoot](../resources/policyroot.md) object.|
|[Update policyRoot](../api/policyroot-update.md)|[policyRoot](../resources/policyroot.md)|Update the properties of a [policyRoot](../resources/policyroot.md) object.|
|[Delete policyRoot](../api/policyroot-delete.md)|None|Deletes a [policyRoot](../resources/policyroot.md) object.|
|[List conditionalAccessPolicies](../api/policyroot-list-conditionalaccesspolicies.md)|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) collection|Get the conditionalAccessPolicies from the conditionalAccessPolicies navigation property.|
|[Create conditionalAccessPolicies](../api/policyroot-post-conditionalaccesspolicies.md)|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)|Create a new conditionalAccessPolicies object.|
|[Get conditionalAccessPolicies](../api/policyroot-get-conditionalaccesspolicy.md)|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)|Read the properties and relationships of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.|
|[Update conditionalAccessPolicies](../api/policyroot-update-conditionalaccesspolicies.md)|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)|Update the properties of a conditionalAccessPolicies object.|
|[Delete conditionalAccessPolicies](../api/policyroot-delete-conditionalaccesspolicies.md)|None|Delete a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.|
|[List identitySecurityDefaultsEnforcementPolicy](../api/policyroot-list-identitysecuritydefaultsenforcementpolicy.md)|[identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) collection|Get the identitySecurityDefaultsEnforcementPolicies from the identitySecurityDefaultsEnforcementPolicy navigation property.|
|[Create identitySecurityDefaultsEnforcementPolicy](../api/policyroot-post-identitysecuritydefaultsenforcementpolicy.md)|[identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md)|Create a new identitySecurityDefaultsEnforcementPolicy object.|
|[Get identitySecurityDefaultsEnforcementPolicy](../api/policyroot-get-identitysecuritydefaultsenforcementpolicy.md)|[identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md)|Read the properties and relationships of an [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object.|
|[Update identitySecurityDefaultsEnforcementPolicy](../api/policyroot-update-identitysecuritydefaultsenforcementpolicy.md)|[identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md)|Update the properties of an identitySecurityDefaultsEnforcementPolicy object.|
|[Delete identitySecurityDefaultsEnforcementPolicy](../api/policyroot-delete-identitysecuritydefaultsenforcementpolicy.md)|None|Delete an [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|activityBasedTimeoutPolicies|[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) collection|**TODO: Add Description**|
|claimsMappingPolicies|[claimsMappingPolicy](../resources/claimsmappingpolicy.md) collection|**TODO: Add Description**|
|conditionalAccessPolicies|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) collection|**TODO: Add Description**|
|homeRealmDiscoveryPolicies|[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) collection|**TODO: Add Description**|
|identitySecurityDefaultsEnforcementPolicy|[identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md)|**TODO: Add Description**|
|tokenIssuancePolicies|[tokenIssuancePolicy](../resources/tokenissuancepolicy.md) collection|**TODO: Add Description**|
|tokenLifetimePolicies|[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policyRoot",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policyRoot",
  "id": "String (identifier)"
}
```

