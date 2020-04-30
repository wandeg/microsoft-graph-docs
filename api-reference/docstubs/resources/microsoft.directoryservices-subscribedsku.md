---
title: "subscribedSku resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# subscribedSku resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List subscribedSkus](../api/microsoft.directoryservices-subscribedsku-list.md)|[subscribedSku](../resources/microsoft.directoryservices-subscribedsku.md) collection|Get a list of the [subscribedSku](../resources/subscribedsku.md) objects and their properties.|
|[Get subscribedSku](../api/microsoft.directoryservices-subscribedsku-get.md)|[subscribedSku](../resources/microsoft.directoryservices-subscribedsku.md)|Read properties and relationships of a [subscribedSku](../resources/microsoft.directoryservices-subscribedsku.md) object.|
|[Create subscribedSku](../api/microsoft.directoryservices-subscribedsku-post-subscribedskus.md)|[subscribedSku](../resources/microsoft.directoryservices-subscribedsku.md)|Create a new [subscribedSku](../resources/microsoft.directoryservices-subscribedsku.md) object.|
|[Delete subscribedSku](../api/microsoft.directoryservices-subscribedsku-delete.md)|None|Deletes a [subscribedSku](../resources/microsoft.directoryservices-subscribedsku.md).|
|[Update subscribedSku](../api/microsoft.directoryservices-subscribedsku-update.md)|[subscribedSku](../resources/microsoft.directoryservices-subscribedsku.md)|Update the properties of a [subscribedSku](../resources/microsoft.directoryservices-subscribedsku.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appliesTo|String|**TODO: Add Description**|
|capabilityStatus|String|**TODO: Add Description**|
|consumedUnits|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|prepaidUnits|[licenseUnitsDetail](../resources/microsoft.directoryservices-licenseunitsdetail.md)|**TODO: Add Description**|
|servicePlans|[servicePlanInfo](../resources/microsoft.directoryservices-serviceplaninfo.md) collection|**TODO: Add Description**|
|skuId|Guid|**TODO: Add Description**|
|skuPartNumber|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.subscribedSku",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.subscribedSku",
  "capabilityStatus": "String",
  "consumedUnits": 1024,
  "id": "String (identifier)",
  "prepaidUnits": {
    "@odata.type": "Microsoft.DirectoryServices.licenseUnitsDetail"
  },
  "servicePlans": [
    {
      "@odata.type": "Microsoft.DirectoryServices.servicePlanInfo"
    }
  ],
  "skuId": "Guid",
  "skuPartNumber": "String",
  "appliesTo": "String"
}
```

