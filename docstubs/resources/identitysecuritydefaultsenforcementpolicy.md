---
title: "identitySecurityDefaultsEnforcementPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# identitySecurityDefaultsEnforcementPolicy resource type


Namespace: microsoft.graph




Inherits from [policyBase](../resources/policybase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get identitySecurityDefaultsEnforcementPolicy](../api/identitysecuritydefaultsenforcementpolicy-get.md)|[identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md)|Read properties and relationships of the [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object.|
|[Update identitySecurityDefaultsEnforcementPolicy](../api/identitysecuritydefaultsenforcementpolicy-update.md)|[identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md)|Update the properties of a [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String| Inherited from [policyBase](../resources/policybase.md)|
|displayName|String| Inherited from [policyBase](../resources/policybase.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|isEnabled|Boolean||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy",
  "baseType": "microsoft.graph.policyBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.identitySecurityDefaultsEnforcementPolicy",
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "isEnabled": true
}
```

