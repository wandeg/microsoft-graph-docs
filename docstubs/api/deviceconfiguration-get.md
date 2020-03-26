---
title: "Get deviceConfiguration"
description: "Read properties and relationships of the deviceConfiguration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get deviceConfiguration

Namespace: microsoft.graph

Read properties and relationships of the [deviceConfiguration](../resources/deviceconfiguration.md) object.

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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [deviceConfiguration](../resources/deviceconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_deviceconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 362

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfiguration",
    "id": "d97af49a-f49a-d97a-9af4-7ad99af47ad9",
    "lastModifiedDateTime": "2016-12-31T23:56:32.7433292+00:00",
    "createdDateTime": "2016-12-31T23:56:38.4791525+00:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```

