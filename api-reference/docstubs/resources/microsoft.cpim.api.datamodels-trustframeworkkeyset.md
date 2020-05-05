---
title: "trustFrameworkKeySet resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# trustFrameworkKeySet resource type


Namespace: microsoft.cpim.api.dataModels

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get trustFrameworkKeySet](../api/microsoft.cpim.api.datamodels-trustframeworkkeyset-get.md)|[trustFrameworkKeySet](../resources/microsoft.cpim.api.datamodels-trustframeworkkeyset.md)|Read properties and relationships of a [trustFrameworkKeySet](../resources/microsoft.cpim.api.datamodels-trustframeworkkeyset.md) object.|
|[Update trustFrameworkKeySet](../api/microsoft.cpim.api.datamodels-trustframeworkkeyset-update.md)|[trustFrameworkKeySet](../resources/microsoft.cpim.api.datamodels-trustframeworkkeyset.md)|Update the properties of a [trustFrameworkKeySet](../resources/microsoft.cpim.api.datamodels-trustframeworkkeyset.md) object.|
|[generateKey](../api/microsoft.cpim.api.datamodels-trustframeworkkeyset-generatekey.md)|[trustFrameworkKey](../resources/microsoft.cpim.api.datamodels-trustframeworkkey.md)|**TODO: Add Description**|
|[uploadSecret](../api/microsoft.cpim.api.datamodels-trustframeworkkeyset-uploadsecret.md)|[trustFrameworkKey](../resources/microsoft.cpim.api.datamodels-trustframeworkkey.md)|**TODO: Add Description**|
|[getActiveKey](../api/microsoft.cpim.api.datamodels-trustframeworkkeyset-getactivekey.md)|[trustFrameworkKey](../resources/microsoft.cpim.api.datamodels-trustframeworkkey.md)|**TODO: Add Description**|
|[uploadCertificate](../api/microsoft.cpim.api.datamodels-trustframeworkkeyset-uploadcertificate.md)|[trustFrameworkKey](../resources/microsoft.cpim.api.datamodels-trustframeworkkey.md)|**TODO: Add Description**|
|[uploadPkcs12](../api/microsoft.cpim.api.datamodels-trustframeworkkeyset-uploadpkcs12.md)|[trustFrameworkKey](../resources/microsoft.cpim.api.datamodels-trustframeworkkey.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|keys|[trustFrameworkKey](../resources/microsoft.cpim.api.datamodels-trustframeworkkey.md) collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.cpim.api.dataModels.trustFrameworkKeySet",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.cpim.api.dataModels.trustFrameworkKeySet",
  "id": "String (identifier)",
  "keys": [
    {
      "@odata.type": "microsoft.cpim.api.dataModels.trustFrameworkKey"
    }
  ]
}
```

