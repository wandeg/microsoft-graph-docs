---
title: "symantecCodeSigningCertificate resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# symantecCodeSigningCertificate resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get symantecCodeSigningCertificate](../api/symanteccodesigningcertificate-get.md)|[symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md)|Read the properties and relationships of a [symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md) object.|
|[Update symantecCodeSigningCertificate](../api/symanteccodesigningcertificate-update.md)|[symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md)|Update the properties of a [symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|Binary|The Windows Symantec Code-Signing Certificate in the raw data format.|
|expirationDateTime|DateTimeOffset|The Cert Expiration Date.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|issuer|String|The Issuer value for the cert.|
|issuerName|String|The Issuer Name for the cert.|
|password|String|The Password required for .pfx file.|
|status|certificateStatus|The Cert Status Provisioned or not Provisioned. Possible values are: `notProvisioned`, `provisioned`.|
|subject|String|The Subject value for the cert.|
|subjectName|String|The Subject Name for the cert.|
|uploadDateTime|DateTimeOffset|The Type of the CodeSigning Cert as Symantec Cert.|

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

