---
title: "trustFrameworkKeySet resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# trustFrameworkKeySet resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get trustFrameworkKeySet](../api/trustframeworkkeyset-get.md)|[trustFrameworkKeySet](../resources/trustFrameworkKeySet.md)|Read properties and relationships of the [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object.|
|[Delete trustFrameworkKeySet](../api/trustframeworkkeyset-delete.md)|None|Deletes a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).|
|[Update trustFrameworkKeySet](../api/trustframeworkkeyset-update.md)|[trustFrameworkKeySet](../resources/trustFrameworkKeySet.md)|Update the properties of a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object.|
|[generateKey](../api/trustframeworkkeyset-generatekey.md)|[trustFrameworkKey](../resources/trustFrameworkKey.md)||
|[uploadSecret](../api/trustframeworkkeyset-uploadsecret.md)|[trustFrameworkKey](../resources/trustFrameworkKey.md)||
|[getActiveKey](../api/trustframeworkkeyset-getactivekey.md)|[trustFrameworkKey](../resources/trustFrameworkKey.md)||
|[uploadCertificate](../api/trustframeworkkeyset-uploadcertificate.md)|[trustFrameworkKey](../resources/trustFrameworkKey.md)||
|[uploadPkcs12](../api/trustframeworkkeyset-uploadpkcs12.md)|[trustFrameworkKey](../resources/trustFrameworkKey.md)||
|[List keySets](../api/trustframework-list-keysets.md)|[trustFrameworkKeySet](../resources/trustFrameworkKeySet.md) collection|Get the trustFrameworkKeySets from the keySets navigation property.|
|[Add keySets](../api/trustframework-post-keysets.md)|[trustFrameworkKeySet](../resources/trustFrameworkKeySet.md)|Add keySets by posting to the keySets collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|keys|[trustFrameworkKey](../resources/trustFrameworkKey.md) collection||

## Relationships
None

## JSON Representation
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

