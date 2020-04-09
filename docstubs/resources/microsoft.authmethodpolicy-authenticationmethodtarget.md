---
title: "authenticationMethodTarget resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# authenticationMethodTarget resource type


Namespace: microsoft.authMethodPolicy



## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get authenticationMethodTarget](../api/microsoft.authmethodpolicy-authenticationmethodtarget-get.md)|[authenticationMethodTarget](../resources/microsoft.authmethodpolicy-authenticationmethodtarget.md)|Read properties and relationships of the [authenticationMethodTarget](../resources/microsoft.authmethodpolicy-authenticationmethodtarget.md) object.|
|[Update authenticationMethodTarget](../api/microsoft.authmethodpolicy-authenticationmethodtarget-update.md)|[authenticationMethodTarget](../resources/microsoft.authmethodpolicy-authenticationmethodtarget.md)|Update the properties of a [authenticationMethodTarget](../resources/microsoft.authmethodpolicy-authenticationmethodtarget.md) object.|
|[List includeTargets](../api/microsoft.authmethodpolicy-authenticationmethodconfiguration-list-includetargets.md)|[authenticationMethodTarget](../resources/microsoft.authmethodpolicy-authenticationmethodtarget.md) collection|Get the authenticationMethodTargets from the includeTargets navigation property.|
|[Add includeTargets](../api/microsoft.authmethodpolicy-authenticationmethodconfiguration-post-includetargets.md)|[authenticationMethodTarget](../resources/microsoft.authmethodpolicy-authenticationmethodtarget.md)|Add includeTargets by posting to the includeTargets collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String||
|isRegistrationRequired|Boolean||
|targetType|Enumeration| Possible values are: `user`, `group`, `unknownFutureValue`.|
|useForSignIn|Boolean||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.authMethodPolicy.authenticationMethodTarget",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.authMethodPolicy.authenticationMethodTarget",
  "targetType": "String",
  "id": "String (identifier)",
  "isRegistrationRequired": true,
  "useForSignIn": true
}
```

