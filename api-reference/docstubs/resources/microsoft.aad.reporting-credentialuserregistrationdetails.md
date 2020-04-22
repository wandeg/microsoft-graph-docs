---
title: "credentialUserRegistrationDetails resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# credentialUserRegistrationDetails resource type


Namespace: Microsoft.AAD.Reporting

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get credentialUserRegistrationDetails](../api/microsoft.aad.reporting-credentialuserregistrationdetails-get.md)|[credentialUserRegistrationDetails](../resources/microsoft.aad.reporting-credentialuserregistrationdetails.md)|Read properties and relationships of a [credentialUserRegistrationDetails](../resources/microsoft.aad.reporting-credentialuserregistrationdetails.md) object.|
|[Update credentialUserRegistrationDetails](../api/microsoft.aad.reporting-credentialuserregistrationdetails-update.md)|[credentialUserRegistrationDetails](../resources/microsoft.aad.reporting-credentialuserregistrationdetails.md)|Update the properties of a [credentialUserRegistrationDetails](../resources/microsoft.aad.reporting-credentialuserregistrationdetails.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|authMethods|registrationAuthMethod collection|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|isCapable|Boolean|**TODO: Add Description**|
|isEnabled|Boolean|**TODO: Add Description**|
|isMfaRegistered|Boolean|**TODO: Add Description**|
|isRegistered|Boolean|**TODO: Add Description**|
|userDisplayName|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.AAD.Reporting.credentialUserRegistrationDetails",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.credentialUserRegistrationDetails",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "userDisplayName": "String",
  "authMethods": [
    "String"
  ],
  "isRegistered": true,
  "isEnabled": true,
  "isCapable": true,
  "isMfaRegistered": true
}
```

