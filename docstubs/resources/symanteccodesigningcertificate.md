---
title: "symantecCodeSigningCertificate resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# symantecCodeSigningCertificate resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get symantecCodeSigningCertificate](../api/symanteccodesigningcertificate-get.md)|[symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md)|Read properties and relationships of the [symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md) object.|
|[Update symantecCodeSigningCertificate](../api/symanteccodesigningcertificate-update.md)|[symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md)|Update the properties of a [symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|Binary||
|expirationDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|issuer|String||
|issuerName|String||
|password|String||
|status|Enumeration| Possible values are: `notProvisioned`, `provisioned`.|
|subject|String||
|subjectName|String||
|uploadDateTime|DateTimeOffset||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.symantecCodeSigningCertificate",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "id": "String (identifier)",
  "content": "binary",
  "status": "String",
  "password": "String",
  "subjectName": "String",
  "subject": "String",
  "issuerName": "String",
  "issuer": "String",
  "expirationDateTime": "String (timestamp)",
  "uploadDateTime": "String (timestamp)"
}
```

