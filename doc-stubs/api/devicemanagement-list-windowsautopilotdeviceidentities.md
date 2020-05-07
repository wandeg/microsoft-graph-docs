---
title: "List windowsAutopilotDeviceIdentities"
description: "Get the windowsAutopilotDeviceIdentities from the windowsAutopilotDeviceIdentities navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List windowsAutopilotDeviceIdentities

Namespace: microsoft.graph

Get the windowsAutopilotDeviceIdentities from the windowsAutopilotDeviceIdentities navigation property.

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
GET /deviceManagement/windowsAutopilotDeviceIdentities
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

If successful, this method returns a `200 OK` response code and a collection of [windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_windowsautopilotdeviceidentity"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.windowsautopilotdeviceidentity)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
      "id": "5ea282ed-82ed-5ea2-ed82-a25eed82a25e",
      "deploymentProfileAssignmentStatus": "String",
      "deploymentProfileAssignmentDetailedStatus": "String",
      "deploymentProfileAssignedDateTime": "String (timestamp)",
      "orderIdentifier": "String",
      "groupTag": "String",
      "purchaseOrderIdentifier": "String",
      "serialNumber": "String",
      "productKey": "String",
      "manufacturer": "String",
      "model": "String",
      "enrollmentState": "String",
      "lastContactedDateTime": "String (timestamp)",
      "addressableUserName": "String",
      "userPrincipalName": "String",
      "resourceName": "String",
      "skuNumber": "String",
      "systemFamily": "String",
      "azureActiveDirectoryDeviceId": "String",
      "managedDeviceId": "String",
      "displayName": "String"
    }
  ]
}
```

