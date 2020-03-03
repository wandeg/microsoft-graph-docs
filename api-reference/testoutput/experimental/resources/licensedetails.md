---
title: "licenseDetails resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# licenseDetails resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get licenseDetails](../api/licensedetails-get.md)|[licenseDetails](../resources/licenseDetails.md)|Read properties and relationships of the [licenseDetails](../resources/licensedetails.md) object.|
|[Delete licenseDetails](../api/licensedetails-delete.md)|None|Deletes a [licenseDetails](../resources/licensedetails.md).|
|[Update licenseDetails](../api/licensedetails-update.md)|[licenseDetails](../resources/licenseDetails.md)|Update the properties of a [licenseDetails](../resources/licensedetails.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|servicePlans|[servicePlanInfo](../resources/servicePlanInfo.md) collection||
|skuId|Guid||
|skuPartNumber|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.licenseDetails",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.licenseDetails",
  "id": "String (identifier)",
  "servicePlans": [
    {
      "@odata.type": "microsoft.graph.servicePlanInfo"
    }
  ],
  "skuId": "Guid",
  "skuPartNumber": "String"
}
```

