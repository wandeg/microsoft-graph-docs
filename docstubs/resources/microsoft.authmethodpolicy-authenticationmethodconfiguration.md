---
title: "authenticationMethodConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# authenticationMethodConfiguration resource type


Namespace: microsoft.authMethodPolicy



## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List authenticationMethodConfigurations](../api/microsoft.authmethodpolicy-authenticationmethodconfiguration-list.md)|[authenticationMethodConfiguration](../resources/microsoft.authmethodpolicy-authenticationmethodconfiguration.md) collection|List properties and relationships of the [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md) objects.|
|[Get authenticationMethodConfiguration](../api/microsoft.authmethodpolicy-authenticationmethodconfiguration-get.md)|[authenticationMethodConfiguration](../resources/microsoft.authmethodpolicy-authenticationmethodconfiguration.md)|Read properties and relationships of the [authenticationMethodConfiguration](../resources/microsoft.authmethodpolicy-authenticationmethodconfiguration.md) object.|
|[List includeTargets](../api/microsoft.authmethodpolicy-authenticationmethodconfiguration-list-includetargets.md)|[authenticationMethodTarget](../resources/microsoft.authmethodpolicy-authenticationmethodtarget.md) collection|Get the authenticationMethodTargets from the includeTargets navigation property.|
|[Add includeTargets](../api/microsoft.authmethodpolicy-authenticationmethodconfiguration-post-includetargets.md)|[authenticationMethodTarget](../resources/microsoft.authmethodpolicy-authenticationmethodtarget.md)|Add includeTargets by posting to the includeTargets collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String||
|state|Enumeration| Possible values are: `enabled`, `disabled`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|includeTargets|[authenticationMethodTarget](../resources/microsoft.authmethodpolicy-authenticationmethodtarget.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.authMethodPolicy.authenticationMethodConfiguration",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.authMethodPolicy.authenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```

