---
title: "credentialUserRegistrationDetails resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# credentialUserRegistrationDetails resource type


Namespace: Microsoft.AAD.Reporting



## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get credentialUserRegistrationDetails](../api/microsoft.aad.reporting-credentialuserregistrationdetails-get.md)|[credentialUserRegistrationDetails](../resources/microsoft.aad.reporting-credentialuserregistrationdetails.md)|Read properties and relationships of the [credentialUserRegistrationDetails](../resources/microsoft.aad.reporting-credentialuserregistrationdetails.md) object.|
|[Update credentialUserRegistrationDetails](../api/microsoft.aad.reporting-credentialuserregistrationdetails-update.md)|[credentialUserRegistrationDetails](../resources/microsoft.aad.reporting-credentialuserregistrationdetails.md)|Update the properties of a [credentialUserRegistrationDetails](../resources/microsoft.aad.reporting-credentialuserregistrationdetails.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|authMethods|Enumeration collection||
|id|String||
|isCapable|Boolean||
|isEnabled|Boolean||
|isMfaRegistered|Boolean||
|isRegistered|Boolean||
|userDisplayName|String||
|userPrincipalName|String||

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

