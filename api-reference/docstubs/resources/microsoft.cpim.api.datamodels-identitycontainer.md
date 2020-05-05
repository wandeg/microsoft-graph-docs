---
title: "identityContainer resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# identityContainer resource type


Namespace: microsoft.cpim.api.dataModels

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get identityContainer](../api/microsoft.cpim.api.datamodels-identitycontainer-get.md)|[identityContainer](../resources/microsoft.cpim.api.datamodels-identitycontainer.md)|Read properties and relationships of an [identityContainer](../resources/microsoft.cpim.api.datamodels-identitycontainer.md) object.|
|[Update identityContainer](../api/microsoft.cpim.api.datamodels-identitycontainer-update.md)|[identityContainer](../resources/microsoft.cpim.api.datamodels-identitycontainer.md)|Update the properties of a [identityContainer](../resources/microsoft.cpim.api.datamodels-identitycontainer.md) object.|
|[List userFlows](../api/microsoft.cpim.api.datamodels-identitycontainer-list-userflows.md)|[identityUserFlow](../resources/microsoft.cpim.api.datamodels-identityuserflow.md) collection|Get the identityUserFlows from the userFlows navigation property.|
|[Create userFlows](../api/microsoft.cpim.api.datamodels-identitycontainer-post-userflows.md)|[identityUserFlow](../resources/microsoft.cpim.api.datamodels-identityuserflow.md)|Create a new userFlows object.|
|[Delete userFlows](../api/microsoft.cpim.api.datamodels-identitycontainer-delete-userflows.md)|None|Delete an userFlows object.|
|[Update userFlows](../api/microsoft.cpim.api.datamodels-identitycontainer-update-userflows.md)|[identityUserFlow](../resources/microsoft.cpim.api.datamodels-identityuserflow.md)|Update the properties of an userFlows object.|
|[Get identityUserFlow](../api/microsoft.cpim.api.datamodels-identityuserflow-get.md)|[identityUserFlow](../resources/microsoft.cpim.api.datamodels-identityuserflow.md)|Read properties and relationships of an [identityUserFlow](../resources/microsoft.cpim.api.datamodels-identityuserflow.md) object.|
|[List featureConfigurations](../api/microsoft.cpim.api.datamodels-identitycontainer-list-featureconfigurations.md)|[featureConfiguration](../resources/microsoft.cpim.api.datamodels-featureconfiguration.md) collection|Get the featureConfigurations from the featureConfigurations navigation property.|
|[Create featureConfigurations](../api/microsoft.cpim.api.datamodels-identitycontainer-post-featureconfigurations.md)|[featureConfiguration](../resources/microsoft.cpim.api.datamodels-featureconfiguration.md)|Create a new featureConfigurations object.|
|[Delete featureConfigurations](../api/microsoft.cpim.api.datamodels-identitycontainer-delete-featureconfigurations.md)|None|Delete a featureConfigurations object.|
|[Update featureConfigurations](../api/microsoft.cpim.api.datamodels-identitycontainer-update-featureconfigurations.md)|[featureConfiguration](../resources/microsoft.cpim.api.datamodels-featureconfiguration.md)|Update the properties of a featureConfigurations object.|
|[Get featureConfiguration](../api/microsoft.cpim.api.datamodels-featureconfiguration-get.md)|[featureConfiguration](../resources/microsoft.cpim.api.datamodels-featureconfiguration.md)|Read properties and relationships of a [featureConfiguration](../resources/microsoft.cpim.api.datamodels-featureconfiguration.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|featureConfigurations|[featureConfiguration](../resources/microsoft.cpim.api.datamodels-featureconfiguration.md) collection|**TODO: Add Description**|
|userFlows|[identityUserFlow](../resources/microsoft.cpim.api.datamodels-identityuserflow.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.cpim.api.dataModels.identityContainer",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.cpim.api.dataModels.identityContainer",
  "id": "String (identifier)"
}
```

