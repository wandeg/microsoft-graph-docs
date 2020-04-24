---
title: "userCredentialUsageDetails resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userCredentialUsageDetails resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userCredentialUsageDetails](../api/usercredentialusagedetails-get.md)|[userCredentialUsageDetails](../resources/usercredentialusagedetails.md)|Read the properties and relationships of a [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) object.|
|[Update userCredentialUsageDetails](../api/usercredentialusagedetails-update.md)|[userCredentialUsageDetails](../resources/usercredentialusagedetails.md)|Update the properties of a [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) object.|
|[List userCredentialUsageDetails](../api/reportroot-list-usercredentialusagedetails.md)|[userCredentialUsageDetails](../resources/usercredentialusagedetails.md) collection|Get the userCredentialUsageDetails from the userCredentialUsageDetails navigation property.|
|[Create userCredentialUsageDetails](../api/reportroot-post-usercredentialusagedetails.md)|[userCredentialUsageDetails](../resources/usercredentialusagedetails.md)|Create a new userCredentialUsageDetails object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|authMethod|usageAuthMethod|**TODO: Add Description**. Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion`, `appNotification`, `appCode`, `alternateMobileCall`, `fido`, `appPassword`, `unknownFutureValue`.|
|eventDateTime|DateTimeOffset|**TODO: Add Description**|
|failureReason|String|**TODO: Add Description**|
|feature|featureType|**TODO: Add Description**. Possible values are: `registration`, `reset`, `unknownFutureValue`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isSuccess|Boolean|**TODO: Add Description**|
|userDisplayName|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|

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

