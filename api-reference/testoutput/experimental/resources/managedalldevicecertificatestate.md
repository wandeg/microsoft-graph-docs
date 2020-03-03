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
|[List managedAllDeviceCertificateStates](../api/managedalldevicecertificatestate-list.md)|[managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md) collection|List properties and relationships of the [managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md) objects.|
|[Get managedAllDeviceCertificateState](../api/managedalldevicecertificatestate-get.md)|[managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md)|Read properties and relationships of the [managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md) object.|
|[Create managedAllDeviceCertificateState](../api/managedalldevicecertificatestate-create.md)|[managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md)|Create a new [managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md) object.|
|[Delete managedAllDeviceCertificateState](../api/managedalldevicecertificatestate-delete.md)|None|Deletes a [managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md).|
|[Update managedAllDeviceCertificateState](../api/managedalldevicecertificatestate-update.md)|[managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md)|Update the properties of a [managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md) object.|
|[List deviceConfigurationsAllManagedDeviceCertificateStates](../api/intune-devices-devicemanagement-list-deviceconfigurationsallmanageddevicecertificatestates.md)|[managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md) collection|Get the managedAllDeviceCertificateStates from the deviceConfigurationsAllManagedDeviceCertificateStates navigation property.|
|[Add deviceConfigurationsAllManagedDeviceCertificateStates](../api/intune-devices-devicemanagement-post-deviceconfigurationsallmanageddevicecertificatestates.md)|[managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md)|Add deviceConfigurationsAllManagedDeviceCertificateStates by posting to the deviceConfigurationsAllManagedDeviceCertificateStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|certificateExpirationDateTime|DateTimeOffset|Certificate expiry date|
|certificateExtendedKeyUsages|String|Enhanced Key Usage|
|certificateIssuanceDateTime|DateTimeOffset|Issuance date|
|certificateIssuerName|String|Issuer|
|certificateKeyUsages|Int32|Key Usage|
|certificateRevokeStatus|Enumeration|Revoke status. Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.|
|certificateSerialNumber|String|Serial number|
|certificateSubjectName|String|Certificate subject name|
|certificateThumbprint|String|Thumbprint|
|id|String| Inherited from [entity](../resources/entity.md)|
|managedDeviceDisplayName|String|Device display name|
|userPrincipalName|String|User principal name|

## Relationships
None

## JSON Representation
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

