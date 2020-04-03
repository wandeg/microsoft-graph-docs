---
title: "List workforceIntegrations"
description: "Get the workforceIntegrations from the workforceIntegrations navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List workforceIntegrations

Namespace: microsoft.graph

Get the workforceIntegrations from the workforceIntegrations navigation property.

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
GET /teamwork/workforceIntegrations
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
If successful, this method returns a `200 OK` response code and a collection of [workforceIntegration](../resources/workforceintegration.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workforceintegration"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/workforceIntegrations
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workforceintegration)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1072

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workforceIntegration",
      "id": "605a42ad-42ad-605a-ad42-5a60ad425a60",
      "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
      "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet",
        "application": {
          "@odata.type": "microsoft.graph.identity",
          "id": "Id value",
          "displayName": "Display Name value"
        },
        "device": {
          "@odata.type": "microsoft.graph.identity"
        },
        "user": {
          "@odata.type": "microsoft.graph.identity"
        }
      },
      "displayName": "Display Name value",
      "apiVersion": 10,
      "encryption": {
        "@odata.type": "microsoft.graph.workforceIntegrationEncryption",
        "protocol": "String",
        "secret": "Secret value"
      },
      "isActive": true,
      "url": "Url value",
      "supports": "String",
      "supportedEntities": "String"
    }
  ]
}
```

