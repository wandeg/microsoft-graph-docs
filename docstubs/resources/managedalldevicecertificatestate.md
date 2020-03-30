---
title: "managedAllDeviceCertificateState resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedAllDeviceCertificateState resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedAllDeviceCertificateState](../api/managedalldevicecertificatestate-get.md)|[managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md)|Read properties and relationships of the [managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md) object.|
|[Update managedAllDeviceCertificateState](../api/managedalldevicecertificatestate-update.md)|[managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md)|Update the properties of a [managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|certificateExpirationDateTime|DateTimeOffset||
|certificateExtendedKeyUsages|String||
|certificateIssuanceDateTime|DateTimeOffset||
|certificateIssuerName|String||
|certificateKeyUsages|Int32||
|certificateRevokeStatus|Enumeration| Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.|
|certificateSerialNumber|String||
|certificateSubjectName|String||
|certificateThumbprint|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|managedDeviceDisplayName|String||
|userPrincipalName|String||

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

