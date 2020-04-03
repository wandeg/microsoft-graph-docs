---
title: "Add deviceConfigurationsAllManagedDeviceCertificateStates"
description: "Add deviceConfigurationsAllManagedDeviceCertificateStates by posting to the deviceConfigurationsAllManagedDeviceCertificateStates collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add deviceConfigurationsAllManagedDeviceCertificateStates

Namespace: microsoft.graph

Add deviceConfigurationsAllManagedDeviceCertificateStates by posting to the deviceConfigurationsAllManagedDeviceCertificateStates collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md) object.

The following table shows the properties that are required when you create the [managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|certificateRevokeStatus|Enumeration| Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.|
|managedDeviceDisplayName|String||
|userPrincipalName|String||
|certificateExpirationDateTime|DateTimeOffset||
|certificateIssuerName|String||
|certificateThumbprint|String||
|certificateSerialNumber|String||
|certificateSubjectName|String||
|certificateKeyUsages|Int32||
|certificateExtendedKeyUsages|String||
|certificateIssuanceDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_managedalldevicecertificatestate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
Content-type: application/json
Content-length: 734

{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "certificateRevokeStatus": "String",
  "managedDeviceDisplayName": "Managed Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "certificateExpirationDateTime": "2017-01-01T00:02:50.9909376+00:00",
  "certificateIssuerName": "Certificate Issuer Name value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateSubjectName": "Certificate Subject Name value",
  "certificateKeyUsages": 4,
  "certificateExtendedKeyUsages": "Certificate Extended Key Usages value",
  "certificateIssuanceDateTime": "2017-01-01T00:00:26.4942185+00:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedalldevicecertificatestate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 783

{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "id": "bb7be305-e305-bb7b-05e3-7bbb05e37bbb",
  "certificateRevokeStatus": "String",
  "managedDeviceDisplayName": "Managed Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "certificateExpirationDateTime": "2017-01-01T00:02:50.9909376+00:00",
  "certificateIssuerName": "Certificate Issuer Name value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateSubjectName": "Certificate Subject Name value",
  "certificateKeyUsages": 4,
  "certificateExtendedKeyUsages": "Certificate Extended Key Usages value",
  "certificateIssuanceDateTime": "2017-01-01T00:00:26.4942185+00:00"
}
```

