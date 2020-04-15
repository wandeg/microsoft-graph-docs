---
title: "userCredentialUsageDetails resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userCredentialUsageDetails resource type


Namespace: Microsoft.AAD.Reporting



## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userCredentialUsageDetails](../api/microsoft.aad.reporting-usercredentialusagedetails-get.md)|[userCredentialUsageDetails](../resources/microsoft.aad.reporting-usercredentialusagedetails.md)|Read properties and relationships of the [userCredentialUsageDetails](../resources/microsoft.aad.reporting-usercredentialusagedetails.md) object.|
|[Update userCredentialUsageDetails](../api/microsoft.aad.reporting-usercredentialusagedetails-update.md)|[userCredentialUsageDetails](../resources/microsoft.aad.reporting-usercredentialusagedetails.md)|Update the properties of a [userCredentialUsageDetails](../resources/microsoft.aad.reporting-usercredentialusagedetails.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|authMethod|Enumeration| Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion`, `appNotification`, `appCode`, `alternateMobileCall`, `fido`, `appPassword`, `unknownFutureValue`.|
|eventDateTime|DateTimeOffset||
|failureReason|String||
|feature|Enumeration| Possible values are: `registration`, `reset`, `unknownFutureValue`.|
|id|String||
|isSuccess|Boolean||
|userDisplayName|String||
|userPrincipalName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.AAD.Reporting.userCredentialUsageDetails",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.userCredentialUsageDetails",
  "id": "String (identifier)",
  "feature": "String",
  "userPrincipalName": "String",
  "userDisplayName": "String",
  "isSuccess": true,
  "authMethod": "String",
  "failureReason": "String",
  "eventDateTime": "String (timestamp)"
}
```

