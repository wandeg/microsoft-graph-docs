---
title: "Get managedAllDeviceCertificateState"
description: "Read the properties and relationships of a managedAllDeviceCertificateState object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get managedAllDeviceCertificateState

Namespace: microsoft.graph

Read the properties and relationships of a [managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md) object.

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
GET /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [managedAllDeviceCertificateState](../resources/managedalldevicecertificatestate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_managedalldevicecertificatestate"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedAllDeviceCertificateState"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
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
}
```

