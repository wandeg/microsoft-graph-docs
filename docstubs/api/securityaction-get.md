---
title: "Get securityAction"
description: "Read properties and relationships of the securityAction object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get securityAction

Namespace: microsoft.graph

Read properties and relationships of the [securityAction](../resources/securityaction.md) object.

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
GET /Security/securityActions/{securityActionId}
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
If successful, this method returns a `200 OK` response code and [securityAction](../resources/securityaction.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_securityaction"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/securityActions/{securityActionId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityAction"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1348

{
  "value": {
    "@odata.type": "#microsoft.graph.securityAction",
    "id": "e4208205-8205-e420-0582-20e4058220e4",
    "actionReason": "Action Reason value",
    "appId": "App Id value",
    "azureTenantId": "Azure Tenant Id value",
    "clientContext": "Client Context value",
    "completedDateTime": "2017-01-01T00:01:37.3404662+03:00",
    "createdDateTime": "2016-12-31T23:57:50.7767122+03:00",
    "errorInfo": {
      "@odata.type": "microsoft.graph.ResultInfo",
      "code": 4,
      "subcode": 7,
      "message": "Message value"
    },
    "lastActionDateTime": "2016-12-31T23:59:45.6080321+03:00",
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
        "updatedDateTime": "2017-01-01T00:02:18.8023442+03:00",
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

