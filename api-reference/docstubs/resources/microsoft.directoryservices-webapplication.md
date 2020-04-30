---
title: "webApplication resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# webApplication resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|homePageUrl|String|**TODO: Add Description**|
|implicitGrantSettings|[implicitGrantSettings](../resources/microsoft.directoryservices-implicitgrantsettings.md)|**TODO: Add Description**|
|logoutUrl|String|**TODO: Add Description**|
|oauth2AllowImplicitFlow|Boolean|**TODO: Add Description**|
|redirectUris|String collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.DirectoryServices.webApplication"
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.webApplication",
  "homePageUrl": "String",
  "redirectUris": [
    "String"
  ],
  "oauth2AllowImplicitFlow": true,
  "logoutUrl": "String",
  "implicitGrantSettings": {
    "@odata.type": "Microsoft.DirectoryServices.implicitGrantSettings",
    "enableIdTokenIssuance": true,
    "enableAccessTokenIssuance": true
  }
}
```

