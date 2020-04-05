---
title: "policyRoot resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# policyRoot resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get policyRoot](../api/policyroot-get.md)|[policyRoot](../resources/policyroot.md)|Read properties and relationships of the [policyRoot](../resources/policyroot.md) object.|
|[Update policyRoot](../api/policyroot-update.md)|[policyRoot](../resources/policyroot.md)|Update the properties of a [policyRoot](../resources/policyroot.md) object.|
|[List activityBasedTimeoutPolicies](../api/policyroot-list-activitybasedtimeoutpolicies.md)|[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) collection|Get the activityBasedTimeoutPolicies from the activityBasedTimeoutPolicies navigation property.|
|[Add activityBasedTimeoutPolicies](../api/policyroot-post-activitybasedtimeoutpolicies.md)|[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)|Add activityBasedTimeoutPolicies by posting to the activityBasedTimeoutPolicies collection.|
|[List claimsMappingPolicies](../api/policyroot-list-claimsmappingpolicies.md)|[claimsMappingPolicy](../resources/claimsmappingpolicy.md) collection|Get the claimsMappingPolicies from the claimsMappingPolicies navigation property.|
|[Add claimsMappingPolicies](../api/policyroot-post-claimsmappingpolicies.md)|[claimsMappingPolicy](../resources/claimsmappingpolicy.md)|Add claimsMappingPolicies by posting to the claimsMappingPolicies collection.|
|[List homeRealmDiscoveryPolicies](../api/policyroot-list-homerealmdiscoverypolicies.md)|[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) collection|Get the homeRealmDiscoveryPolicies from the homeRealmDiscoveryPolicies navigation property.|
|[Add homeRealmDiscoveryPolicies](../api/policyroot-post-homerealmdiscoverypolicies.md)|[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)|Add homeRealmDiscoveryPolicies by posting to the homeRealmDiscoveryPolicies collection.|
|[List tokenIssuancePolicies](../api/policyroot-list-tokenissuancepolicies.md)|[tokenIssuancePolicy](../resources/tokenissuancepolicy.md) collection|Get the tokenIssuancePolicies from the tokenIssuancePolicies navigation property.|
|[Add tokenIssuancePolicies](../api/policyroot-post-tokenissuancepolicies.md)|[tokenIssuancePolicy](../resources/tokenissuancepolicy.md)|Add tokenIssuancePolicies by posting to the tokenIssuancePolicies collection.|
|[List tokenLifetimePolicies](../api/policyroot-list-tokenlifetimepolicies.md)|[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) collection|Get the tokenLifetimePolicies from the tokenLifetimePolicies navigation property.|
|[Add tokenLifetimePolicies](../api/policyroot-post-tokenlifetimepolicies.md)|[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)|Add tokenLifetimePolicies by posting to the tokenLifetimePolicies collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|activityBasedTimeoutPolicies|[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) collection||
|claimsMappingPolicies|[claimsMappingPolicy](../resources/claimsmappingpolicy.md) collection||
|homeRealmDiscoveryPolicies|[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) collection||
|tokenIssuancePolicies|[tokenIssuancePolicy](../resources/tokenissuancepolicy.md) collection||
|tokenLifetimePolicies|[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) collection||

## JSON representation
Here is a JSON representation of the resource.
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

