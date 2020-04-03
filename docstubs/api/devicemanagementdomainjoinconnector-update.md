---
title: "Update deviceManagementDomainJoinConnector"
description: "Update the properties of a deviceManagementDomainJoinConnector object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceManagementDomainJoinConnector

Namespace: microsoft.graph

Update the properties of a [deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md) object.

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
PATCH /deviceManagement/domainJoinConnectors/{deviceManagementDomainJoinConnectorId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md) object.

The following table shows the properties that are required when you create the [deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|lastConnectionDateTime|DateTimeOffset||
|state|Enumeration| Possible values are: `active`, `error`, `inactive`.|
|version|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementdomainjoinconnector"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/domainJoinConnectors/{deviceManagementDomainJoinConnectorId}
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "displayName": "Display Name value",
  "lastConnectionDateTime": "2017-01-01T00:01:57.2663846+00:00",
  "state": "String",
  "version": "Version value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "id": "87679931-9931-8767-3199-678731996787",
  "displayName": "Display Name value",
  "lastConnectionDateTime": "2017-01-01T00:01:57.2663846+00:00",
  "state": "String",
  "version": "Version value"
}
```

