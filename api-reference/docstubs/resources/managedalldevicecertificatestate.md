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


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedAllDeviceCertificateState](../api/managedalldevicecertificatestate-get.md)|[managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md)|Read the properties and relationships of a [managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md) object.|
|[Update managedAllDeviceCertificateState](../api/managedalldevicecertificatestate-update.md)|[managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md)|Update the properties of a [managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|certificateExpirationDateTime|DateTimeOffset|Certificate expiry date|
|certificateExtendedKeyUsages|String|Enhanced Key Usage|
|certificateIssuanceDateTime|DateTimeOffset|Issuance date|
|certificateIssuerName|String|Issuer|
|certificateKeyUsages|Int32|Key Usage|
|certificateRevokeStatus|certificateRevocationStatus|Revoke status. Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.|
|certificateSerialNumber|String|Serial number|
|certificateSubjectName|String|Certificate subject name|
|certificateThumbprint|String|Thumbprint|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|managedDeviceDisplayName|String|Device display name|
|userPrincipalName|String|User principal name|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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
  "certificateKeyUsages": 1024,
  "certificateExtendedKeyUsages": "String",
  "certificateIssuanceDateTime": "String (timestamp)"
}
```

