---
title: "certificateAuthority resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# certificateAuthority resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|certificate|Binary|**TODO: Add Description**|
|certificateRevocationListUrl|String|**TODO: Add Description**|
|deltaCertificateRevocationListUrl|String|**TODO: Add Description**|
|isRootAuthority|Boolean|**TODO: Add Description**|
|issuer|String|**TODO: Add Description**|
|issuerSki|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.certificateAuthority"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateAuthority",
  "isRootAuthority": true,
  "certificateRevocationListUrl": "String",
  "deltaCertificateRevocationListUrl": "String",
  "certificate": "binary",
  "issuer": "String",
  "issuerSki": "String"
}
```

