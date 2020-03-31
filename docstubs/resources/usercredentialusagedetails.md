---
title: "userCredentialUsageDetails resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userCredentialUsageDetails resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userCredentialUsageDetails](../api/usercredentialusagedetails-get.md)|[userCredentialUsageDetails](../resources/usercredentialusagedetails.md)|Read properties and relationships of the [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) object.|
|[Update userCredentialUsageDetails](../api/usercredentialusagedetails-update.md)|[userCredentialUsageDetails](../resources/usercredentialusagedetails.md)|Update the properties of a [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|authMethod|Enumeration| Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion`, `appNotification`, `appCode`, `alternateMobileCall`, `fido`, `appPassword`, `unknownFutureValue`.|
|eventDateTime|DateTimeOffset||
|failureReason|String||
|feature|Enumeration| Possible values are: `registration`, `reset`, `unknownFutureValue`.|
|id|String| Inherited from [entity](../resources/entity.md)|
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
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userCredentialUsageDetails",
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

