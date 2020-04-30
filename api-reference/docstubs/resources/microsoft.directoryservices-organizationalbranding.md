---
title: "organizationalBranding resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# organizationalBranding resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get organizationalBranding](../api/microsoft.directoryservices-organizationalbranding-get.md)|[organizationalBranding](../resources/microsoft.directoryservices-organizationalbranding.md)|Read properties and relationships of an [organizationalBranding](../resources/microsoft.directoryservices-organizationalbranding.md) object.|
|[Update organizationalBranding](../api/microsoft.directoryservices-organizationalbranding-update.md)|[organizationalBranding](../resources/microsoft.directoryservices-organizationalbranding.md)|Update the properties of a [organizationalBranding](../resources/microsoft.directoryservices-organizationalbranding.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|backgroundColor|String|**TODO: Add Description**|
|backgroundImage|Stream|**TODO: Add Description**|
|bannerLogo|Stream|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|locale|String|**TODO: Add Description**|
|signInPageText|String|**TODO: Add Description**|
|squareLogo|Stream|**TODO: Add Description**|
|usernameHintText|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.organizationalBranding",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.organizationalBranding",
  "id": "String (identifier)",
  "backgroundColor": "String",
  "backgroundImage": "Stream",
  "bannerLogo": "Stream",
  "locale": "String",
  "signInPageText": "String",
  "squareLogo": "Stream",
  "usernameHintText": "String"
}
```

