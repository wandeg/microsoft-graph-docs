---
title: "List securityActions"
description: "Get the securityActions from the securityActions navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List securityActions

Namespace: microsoft.graph

Get the securityActions from the securityActions navigation property.

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
GET /Security/securityActions
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

If successful, this method returns a `200 OK` response code and a collection of [securityAction](../resources/securityaction.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_securityaction"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/securityActions
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.securityaction)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.securityAction",
      "id": "3d4209eb-09eb-3d42-eb09-423deb09423d",
      "actionReason": "String",
      "appId": "String",
      "azureTenantId": "String",
      "clientContext": "String",
      "completedDateTime": "String (timestamp)",
      "createdDateTime": "String (timestamp)",
      "errorInfo": {
        "@odata.type": "microsoft.graph.ResultInfo"
      },
      "lastActionDateTime": "String (timestamp)",
      "name": "String",
      "parameters": [
        {
          "@odata.type": "microsoft.graph.keyValuePair"
        }
      ],
      "states": [
        {
          "@odata.type": "microsoft.graph.securityActionState"
        }
      ],
      "status": "String",
      "user": "String",
      "vendorInformation": {
        "@odata.type": "microsoft.graph.securityVendorInformation"
      }
    }
  ]
}
```

