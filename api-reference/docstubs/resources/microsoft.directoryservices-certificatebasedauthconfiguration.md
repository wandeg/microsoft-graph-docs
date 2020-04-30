---
title: "certificateBasedAuthConfiguration resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# certificateBasedAuthConfiguration resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get certificateBasedAuthConfiguration](../api/microsoft.directoryservices-certificatebasedauthconfiguration-get.md)|[certificateBasedAuthConfiguration](../resources/microsoft.directoryservices-certificatebasedauthconfiguration.md)|Read properties and relationships of a [certificateBasedAuthConfiguration](../resources/microsoft.directoryservices-certificatebasedauthconfiguration.md) object.|
|[Update certificateBasedAuthConfiguration](../api/microsoft.directoryservices-certificatebasedauthconfiguration-update.md)|[certificateBasedAuthConfiguration](../resources/microsoft.directoryservices-certificatebasedauthconfiguration.md)|Update the properties of a [certificateBasedAuthConfiguration](../resources/microsoft.directoryservices-certificatebasedauthconfiguration.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|certificateAuthorities|[certificateAuthority](../resources/microsoft.directoryservices-certificateauthority.md) collection|**TODO: Add Description**|
|id|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.certificateBasedAuthConfiguration",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.certificateBasedAuthConfiguration",
  "id": "String (identifier)",
  "certificateAuthorities": [
    {
      "@odata.type": "Microsoft.DirectoryServices.certificateAuthority"
    }
  ]
}
```

