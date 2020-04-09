---
title: "authenticationMethodsPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# authenticationMethodsPolicy resource type


Namespace: microsoft.authMethodPolicy



## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get authenticationMethodsPolicy](../api/microsoft.authmethodpolicy-authenticationmethodspolicy-get.md)|[authenticationMethodsPolicy](../resources/microsoft.authmethodpolicy-authenticationmethodspolicy.md)|Read properties and relationships of the [authenticationMethodsPolicy](../resources/microsoft.authmethodpolicy-authenticationmethodspolicy.md) object.|
|[Update authenticationMethodsPolicy](../api/microsoft.authmethodpolicy-authenticationmethodspolicy-update.md)|[authenticationMethodsPolicy](../resources/microsoft.authmethodpolicy-authenticationmethodspolicy.md)|Update the properties of a [authenticationMethodsPolicy](../resources/microsoft.authmethodpolicy-authenticationmethodspolicy.md) object.|
|[List authenticationMethodConfigurations](../api/microsoft.authmethodpolicy-authenticationmethodspolicy-list-authenticationmethodconfigurations.md)|[authenticationMethodConfiguration](../resources/microsoft.authmethodpolicy-authenticationmethodconfiguration.md) collection|Get the authenticationMethodConfigurations from the authenticationMethodConfigurations navigation property.|
|[Add authenticationMethodConfigurations](../api/microsoft.authmethodpolicy-authenticationmethodspolicy-post-authenticationmethodconfigurations.md)|[authenticationMethodConfiguration](../resources/microsoft.authmethodpolicy-authenticationmethodconfiguration.md)|Add authenticationMethodConfigurations by posting to the authenticationMethodConfigurations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|convergedPolicyTargetGroup|String||
|description|String||
|displayName|String||
|id|String||
|lastModifiedDateTime|DateTimeOffset||
|policyVersion|String||
|reconfirmationInDays|Int32||
|registrationAndResetTargets|[registrationAndResetTarget](../resources/microsoft.authmethodpolicy-registrationandresettarget.md) collection||
|registrationEnforcement|[registrationEnforcement](../resources/microsoft.authmethodpolicy-registrationenforcement.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|authenticationMethodConfigurations|[authenticationMethodConfiguration](../resources/microsoft.authmethodpolicy-authenticationmethodconfiguration.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.authMethodPolicy.authenticationMethodsPolicy",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.authMethodPolicy.authenticationMethodsPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "policyVersion": "String",
  "convergedPolicyTargetGroup": "String",
  "registrationAndResetTargets": [
    {
      "@odata.type": "microsoft.authMethodPolicy.registrationAndResetTarget",
      "id": "String",
      "minAuthMethodsToRegister": 1024,
      "minAuthMethodsToReset": 1024
    }
  ],
  "registrationEnforcement": {
    "@odata.type": "microsoft.authMethodPolicy.registrationEnforcement",
    "isAllowedToSkipRegistration": true,
    "registrationSkipDurationInDays": 1024
  },
  "reconfirmationInDays": 1024
}
```

