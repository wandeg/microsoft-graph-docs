---
title: "managedAllDeviceCertificateState resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedAllDeviceCertificateState resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|certificateExpirationDateTime|DateTimeOffset|**TODO: Add Description**|
|certificateExtendedKeyUsages|String|**TODO: Add Description**|
|certificateIssuanceDateTime|DateTimeOffset|**TODO: Add Description**|
|certificateIssuerName|String|**TODO: Add Description**|
|certificateKeyUsages|Int32|**TODO: Add Description**|
|certificateRevokeStatus|certificateRevocationStatus|**TODO: Add Description**. Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.|
|certificateSerialNumber|String|**TODO: Add Description**|
|certificateSubjectName|String|**TODO: Add Description**|
|certificateThumbprint|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|managedDeviceDisplayName|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAllDeviceCertificateState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "id": "String (identifier)",
  "certificateRevokeStatus": "String",
  "managedDeviceDisplayName": "String",
  "userPrincipalName": "String",
  "certificateExpirationDateTime": "String (timestamp)",
  "certificateIssuerName": "String",
  "certificateThumbprint": "String",
  "certificateSerialNumber": "String",
  "certificateSubjectName": "String",
  "certificateKeyUsages": "Integer",
  "certificateExtendedKeyUsages": "String",
  "certificateIssuanceDateTime": "String (timestamp)"
}
```

