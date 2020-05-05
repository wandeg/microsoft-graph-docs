---
title: "identityProvider resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# identityProvider resource type


Namespace: microsoft.cpim.api.dataModels

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List identityProviders](../api/microsoft.cpim.api.datamodels-identityprovider-list.md)|[identityProvider](../resources/microsoft.cpim.api.datamodels-identityprovider.md) collection|Get a list of the [identityProvider](../resources/identityprovider.md) objects and their properties.|
|[Get identityProvider](../api/microsoft.cpim.api.datamodels-identityprovider-get.md)|[identityProvider](../resources/microsoft.cpim.api.datamodels-identityprovider.md)|Read properties and relationships of an [identityProvider](../resources/microsoft.cpim.api.datamodels-identityprovider.md) object.|
|[Create identityProvider](../api/microsoft.cpim.api.datamodels-identityprovider-post-identityproviders.md)|[identityProvider](../resources/microsoft.cpim.api.datamodels-identityprovider.md)|Create a new [identityProvider](../resources/microsoft.cpim.api.datamodels-identityprovider.md) object.|
|[Delete identityProvider](../api/microsoft.cpim.api.datamodels-identityprovider-delete.md)|None|Deletes an [identityProvider](../resources/microsoft.cpim.api.datamodels-identityprovider.md).|
|[Update identityProvider](../api/microsoft.cpim.api.datamodels-identityprovider-update.md)|[identityProvider](../resources/microsoft.cpim.api.datamodels-identityprovider.md)|Update the properties of a [identityProvider](../resources/microsoft.cpim.api.datamodels-identityprovider.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|clientId|String|**TODO: Add Description**|
|clientSecret|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.cpim.api.dataModels.identityProvider",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.cpim.api.dataModels.identityProvider",
  "id": "String (identifier)",
  "type": "String",
  "name": "String",
  "clientId": "String",
  "clientSecret": "String"
}
```

