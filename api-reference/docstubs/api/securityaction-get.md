---
title: "Get securityAction"
description: "Read the properties and relationships of a securityAction object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get securityAction

Namespace: microsoft.graph

Read the properties and relationships of a [securityAction](../resources/securityaction.md) object.

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
GET /Security/securityActions/{securityActionId}
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
If successful, this method returns a `200 OK` response code and a [securityAction](../resources/securityaction.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_securityaction"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/securityActions/{securityActionId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityAction"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.securityAction",
    "id": "cf3a5d69-5d69-cf3a-695d-3acf695d3acf",
    "actionReason": "Action Reason value",
    "appId": "App Id value",
    "azureTenantId": "Azure Tenant Id value",
    "clientContext": "Client Context value",
    "completedDateTime": "2017-01-01T00:02:03.9770517+03:00",
    "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
    "errorInfo": {
      "@odata.type": "microsoft.graph.ResultInfo",
      "code": 4,
      "subcode": 7,
      "message": "Message value"
    },
    "lastActionDateTime": "2016-12-31T23:57:13.8078619+03:00",
    "name": "Name value",
    "parameters": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "value": "Value value"
      }
    ],
    "states": [
      {
        "@odata.type": "microsoft.graph.securityActionState",
        "status": "String",
        "updatedDateTime": "2017-01-01T00:00:22.114869+03:00",
        "user": "User value"
      }
    ],
    "status": "String",
    "user": "User value",
    "vendorInformation": {
      "@odata.type": "microsoft.graph.securityVendorInformation",
      "provider": "Provider value",
      "providerVersion": "Provider Version value",
      "subProvider": "Sub Provider value",
      "vendor": "Vendor value"
    }
  }
}
```

