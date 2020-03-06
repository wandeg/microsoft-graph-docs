---
title: "enterpriseCodeSigningCertificate resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# enterpriseCodeSigningCertificate resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get enterpriseCodeSigningCertificate](../api/enterprisecodesigningcertificate-get.md)|[enterpriseCodeSigningCertificate](../resources/enterprisecodesigningcertificate.md)|Read properties and relationships of the [enterpriseCodeSigningCertificate](../resources/enterprisecodesigningcertificate.md) object.|
|[Update enterpriseCodeSigningCertificate](../api/enterprisecodesigningcertificate-update.md)|[enterpriseCodeSigningCertificate](../resources/enterprisecodesigningcertificate.md)|Update the properties of a [enterpriseCodeSigningCertificate](../resources/enterprisecodesigningcertificate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|Binary|The Windows Enterprise Code-Signing Certificate in the raw data format.|
|expirationDateTime|DateTimeOffset|The Cert Expiration Date.|
|id|String| Inherited from [entity](../resources/entity.md)|
|issuer|String|The Issuer value for the cert.|
|issuerName|String|The Issuer Name for the cert.|
|status|Enumeration|The Certificate Status Provisioned or not Provisioned. Possible values are: `notProvisioned`, `provisioned`.|
|subject|String|The Subject Value for the cert.|
|subjectName|String|The Subject Name for the cert.|
|uploadDateTime|DateTimeOffset|The date time of CodeSigning Cert when it is uploaded.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enterpriseCodeSigningCertificate",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "id": "String (identifier)",
  "content": "binary",
  "status": "String",
  "subjectName": "String",
  "subject": "String",
  "issuerName": "String",
  "issuer": "String",
  "expirationDateTime": "String (timestamp)",
  "uploadDateTime": "String (timestamp)"
}
```

