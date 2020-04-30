---
title: "licenseDetails resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# licenseDetails resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get licenseDetails](../api/microsoft.directoryservices-licensedetails-get.md)|[licenseDetails](../resources/microsoft.directoryservices-licensedetails.md)|Read properties and relationships of a [licenseDetails](../resources/microsoft.directoryservices-licensedetails.md) object.|
|[Update licenseDetails](../api/microsoft.directoryservices-licensedetails-update.md)|[licenseDetails](../resources/microsoft.directoryservices-licensedetails.md)|Update the properties of a [licenseDetails](../resources/microsoft.directoryservices-licensedetails.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
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
  "@odata.type": "Microsoft.DirectoryServices.licenseDetails",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.licenseDetails",
  "id": "String (identifier)",
  "servicePlans": [
    {
      "@odata.type": "Microsoft.DirectoryServices.servicePlanInfo"
    }
  ],
  "skuId": "Guid",
  "skuPartNumber": "String"
}
```

