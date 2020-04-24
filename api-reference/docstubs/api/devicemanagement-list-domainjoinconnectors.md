---
title: "List domainJoinConnectors"
description: "Get the deviceManagementDomainJoinConnectors from the domainJoinConnectors navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List domainJoinConnectors

Namespace: microsoft.graph

Get the deviceManagementDomainJoinConnectors from the domainJoinConnectors navigation property.

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
GET /deviceManagement/domainJoinConnectors
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
If successful, this method returns a `200 OK` response code and a collection of [deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementdomainjoinconnector"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/domainJoinConnectors
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicemanagementdomainjoinconnector)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
      "id": "39d5be50-be50-39d5-50be-d53950bed539",
      "displayName": "Display Name value",
      "lastConnectionDateTime": "2016-12-31T23:57:28.9541214+03:00",
      "state": "String",
      "version": "Version value"
    }
  ]
}
```

