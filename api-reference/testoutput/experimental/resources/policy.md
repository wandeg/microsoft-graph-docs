---
title: "policy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# policy resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get policy](../api/policy-get.md)|[policy](../resources/policy.md)|Read properties and relationships of the [policy](../resources/policy.md) object.|
|[Update policy](../api/policy-update.md)|[policy](../resources/policy.md)|Update the properties of a [policy](../resources/policy.md) object.|
|[List activityBasedTimeoutPolicies](../api/policy-list-activitybasedtimeoutpolicies.md)|[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) collection|Get the activityBasedTimeoutPolicies from the activityBasedTimeoutPolicies navigation property.|
|[Add activityBasedTimeoutPolicies](../api/policy-post-activitybasedtimeoutpolicies.md)|[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)|Add activityBasedTimeoutPolicies by posting to the activityBasedTimeoutPolicies collection.|
|[List claimsMappingPolicies](../api/policy-list-claimsmappingpolicies.md)|[claimsMappingPolicy](../resources/claimsmappingpolicy.md) collection|Get the claimsMappingPolicies from the claimsMappingPolicies navigation property.|
|[Add claimsMappingPolicies](../api/policy-post-claimsmappingpolicies.md)|[claimsMappingPolicy](../resources/claimsmappingpolicy.md)|Add claimsMappingPolicies by posting to the claimsMappingPolicies collection.|
|[List homeRealmDiscoveryPolicies](../api/policy-list-homerealmdiscoverypolicies.md)|[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) collection|Get the homeRealmDiscoveryPolicies from the homeRealmDiscoveryPolicies navigation property.|
|[Add homeRealmDiscoveryPolicies](../api/policy-post-homerealmdiscoverypolicies.md)|[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)|Add homeRealmDiscoveryPolicies by posting to the homeRealmDiscoveryPolicies collection.|
|[List tokenLifetimePolicies](../api/policy-list-tokenlifetimepolicies.md)|[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) collection|Get the tokenLifetimePolicies from the tokenLifetimePolicies navigation property.|
|[Add tokenLifetimePolicies](../api/policy-post-tokenlifetimepolicies.md)|[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)|Add tokenLifetimePolicies by posting to the tokenLifetimePolicies collection.|

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
|tokenLifetimePolicies|[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policy",
  "id": "String (identifier)"
}
```

