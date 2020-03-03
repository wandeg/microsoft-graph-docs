---
title: "iosVpnSecurityAssociationParameters resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# iosVpnSecurityAssociationParameters resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|lifetimeInMinutes|Int32|Lifetime (minutes)|
|securityDiffieHellmanGroup|Int32|Diffie-Hellman Group|
|securityEncryptionAlgorithm|Enumeration|Encryption algorithm. Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`.|
|securityIntegrityAlgorithm|Enumeration|Integrity algorithm. Possible values are: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVpnSecurityAssociationParameters",
  "securityEncryptionAlgorithm": "String",
  "securityIntegrityAlgorithm": "String",
  "securityDiffieHellmanGroup": 1024,
  "lifetimeInMinutes": 1024
}
```

