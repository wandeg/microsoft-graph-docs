---
title: "trustFrameworkKeySet resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# trustFrameworkKeySet resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get trustFrameworkKeySet](../api/trustframeworkkeyset-get.md)|[trustFrameworkKeySet](../resources/trustframeworkkeyset.md)|Read properties and relationships of the [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object.|
|[Update trustFrameworkKeySet](../api/trustframeworkkeyset-update.md)|[trustFrameworkKeySet](../resources/trustframeworkkeyset.md)|Update the properties of a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object.|
|[generateKey](../api/trustframeworkkeyset-generatekey.md)|[trustFrameworkKey](../resources/trustframeworkkey.md)||
|[uploadSecret](../api/trustframeworkkeyset-uploadsecret.md)|[trustFrameworkKey](../resources/trustframeworkkey.md)||
|[getActiveKey](../api/trustframeworkkeyset-getactivekey.md)|[trustFrameworkKey](../resources/trustframeworkkey.md)||
|[uploadCertificate](../api/trustframeworkkeyset-uploadcertificate.md)|[trustFrameworkKey](../resources/trustframeworkkey.md)||
|[uploadPkcs12](../api/trustframeworkkeyset-uploadpkcs12.md)|[trustFrameworkKey](../resources/trustframeworkkey.md)||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|keys|[trustFrameworkKey](../resources/trustframeworkkey.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.trustFrameworkKeySet",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.trustFrameworkKeySet",
  "id": "String (identifier)",
  "keys": [
    {
      "@odata.type": "microsoft.graph.trustFrameworkKey"
    }
  ]
}
```

