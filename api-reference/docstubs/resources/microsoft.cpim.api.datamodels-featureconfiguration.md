---
title: "featureConfiguration resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# featureConfiguration resource type


Namespace: microsoft.cpim.api.dataModels

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get featureConfiguration](../api/microsoft.cpim.api.datamodels-featureconfiguration-get.md)|[featureConfiguration](../resources/microsoft.cpim.api.datamodels-featureconfiguration.md)|Read properties and relationships of a [featureConfiguration](../resources/microsoft.cpim.api.datamodels-featureconfiguration.md) object.|
|[Update featureConfiguration](../api/microsoft.cpim.api.datamodels-featureconfiguration-update.md)|[featureConfiguration](../resources/microsoft.cpim.api.datamodels-featureconfiguration.md)|Update the properties of a [featureConfiguration](../resources/microsoft.cpim.api.datamodels-featureconfiguration.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activatedFeatureTiers|identityFeatureTier|**TODO: Add Description**. Possible values are: `Standard`, `PremiumP1`, `PremiumP2`, `unknownFutureValue`.|
|azureResourceGroupName|String|**TODO: Add Description**|
|azureResourceName|String|**TODO: Add Description**|
|azureSubscriptionId|String|**TODO: Add Description**|
|azureSubscriptionTenantId|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.cpim.api.dataModels.featureConfiguration",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.cpim.api.dataModels.featureConfiguration",
  "id": "String (identifier)",
  "activatedFeatureTiers": "String",
  "azureResourceGroupName": "String",
  "azureResourceName": "String",
  "azureSubscriptionId": "String",
  "azureSubscriptionTenantId": "String"
}
```

