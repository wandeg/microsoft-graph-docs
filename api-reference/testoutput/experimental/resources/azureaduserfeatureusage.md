---
title: "azureADUserFeatureUsage resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# azureADUserFeatureUsage resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List azureADUserFeatureUsages](../api/azureaduserfeatureusage-list.md)|[azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md) collection|List properties and relationships of the [azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md) objects.|
|[Get azureADUserFeatureUsage](../api/azureaduserfeatureusage-get.md)|[azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md)|Read properties and relationships of the [azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md) object.|
|[Create azureADUserFeatureUsage](../api/azureaduserfeatureusage-create.md)|[azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md)|Create a new [azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md) object.|
|[Delete azureADUserFeatureUsage](../api/azureaduserfeatureusage-delete.md)|None|Deletes a [azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md).|
|[Update azureADUserFeatureUsage](../api/azureaduserfeatureusage-update.md)|[azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md)|Update the properties of a [azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|featureUsageDetails|[featureUsageDetail](../resources/featureusagedetail.md) collection||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastUpdatedDateTime|DateTimeOffset||
|licenseAssigned|Enumeration|. Possible values are: `none`, `free`, `basic`, `premiumP1`, `premiumP2`, `unknownFutureValue`.|
|licenseRecommended|Enumeration|. Possible values are: `none`, `free`, `basic`, `premiumP1`, `premiumP2`, `unknownFutureValue`.|
|userDisplayName|String||
|userId|String||
|userPrincipalName|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.azureADUserFeatureUsage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.azureADUserFeatureUsage",
  "id": "String (identifier)",
  "lastUpdatedDateTime": "String (timestamp)",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "licenseRecommended": "String",
  "licenseAssigned": "String",
  "featureUsageDetails": [
    {
      "@odata.type": "microsoft.graph.featureUsageDetail"
    }
  ]
}
```

