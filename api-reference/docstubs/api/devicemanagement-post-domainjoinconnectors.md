---
title: "Create domainJoinConnectors"
description: "Create a new domainJoinConnectors object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create domainJoinConnectors

Namespace: microsoft.graph

Create a new domainJoinConnectors object.

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
POST /deviceManagement/domainJoinConnectors
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md) object.

The following table shows the properties that are required when you create the [deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|The connector display name.|
|lastConnectionDateTime|DateTimeOffset|Last time connector contacted Intune.|
|state|deviceManagementDomainJoinConnectorState|The connector state. Possible values are: `active`, `error`, `inactive`.|
|version|String|The version of the connector.|



## Response
If successful, this method returns a `201 Created` response code and a [deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementdomainjoinconnector_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/domainJoinConnectors
Content-Type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "displayName": "Display Name value",
  "lastConnectionDateTime": "2016-12-31T23:57:28.9541214+03:00",
  "state": "String",
  "version": "Version value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementdomainjoinconnector"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "id": "39d5be50-be50-39d5-50be-d53950bed539",
  "displayName": "Display Name value",
  "lastConnectionDateTime": "2016-12-31T23:57:28.9541214+03:00",
  "state": "String",
  "version": "Version value"
}
```

