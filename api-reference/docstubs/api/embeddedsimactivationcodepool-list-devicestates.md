---
title: "List deviceStates"
description: "Get the embeddedSIMDeviceStates from the deviceStates navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List deviceStates

Namespace: microsoft.graph

Get the embeddedSIMDeviceStates from the deviceStates navigation property.

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
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_embeddedsimdevicestate"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.embeddedsimdevicestate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
      "id": "8d88956d-956d-8d88-6d95-888d6d95888d",
      "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
      "modifiedDateTime": "2017-01-01T00:00:03.7977786+03:00",
      "lastSyncDateTime": "2017-01-01T00:02:17.5414184+03:00",
      "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
      "deviceName": "Device Name value",
      "userName": "User Name value",
      "state": "String",
      "stateDetails": "State Details value"
    }
  ]
}
```

