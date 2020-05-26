---
title: "verifiedCustomDomainCertificatesMetadata resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# verifiedCustomDomainCertificatesMetadata resource type

Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|expiryDate|DateTimeOffset|**TODO: Add Description**|
|issueDate|DateTimeOffset|**TODO: Add Description**|
|issuerName|String|**TODO: Add Description**|
|subjectName|String|**TODO: Add Description**|
|thumbprint|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.verifiedCustomDomainCertificatesMetadata"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.verifiedCustomDomainCertificatesMetadata",
  "thumbprint": "String",
  "subjectName": "String",
  "issuerName": "String",
  "issueDate": "String (timestamp)",
  "expiryDate": "String (timestamp)"
}
```

