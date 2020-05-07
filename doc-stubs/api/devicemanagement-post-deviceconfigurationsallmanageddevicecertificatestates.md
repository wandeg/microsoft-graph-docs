---
title: "Create deviceConfigurationsAllManagedDeviceCertificateStates"
description: "Create a new deviceConfigurationsAllManagedDeviceCertificateStates object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create deviceConfigurationsAllManagedDeviceCertificateStates

Namespace: microsoft.graph

Create a new deviceConfigurationsAllManagedDeviceCertificateStates object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md) object.

The following table shows the properties that are required when you create the [managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|certificateRevokeStatus|certificateRevocationStatus|**TODO: Add Description**. Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.|
|managedDeviceDisplayName|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|
|certificateExpirationDateTime|DateTimeOffset|**TODO: Add Description**|
|certificateIssuerName|String|**TODO: Add Description**|
|certificateThumbprint|String|**TODO: Add Description**|
|certificateSerialNumber|String|**TODO: Add Description**|
|certificateSubjectName|String|**TODO: Add Description**|
|certificateKeyUsages|Int32|**TODO: Add Description**|
|certificateExtendedKeyUsages|String|**TODO: Add Description**|
|certificateIssuanceDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_managedalldevicecertificatestate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
Content-Type: application/json
Content-length: 541

{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
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

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedalldevicecertificatestate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "id": "20015051-5051-2001-5150-012051500120",
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

