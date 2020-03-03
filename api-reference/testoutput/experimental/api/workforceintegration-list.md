---
title: "List workforceIntegrations"
description: "List properties and relationships of the workforceIntegration objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List workforceIntegrations

Namespace: microsoft.graph

List properties and relationships of the [workforceIntegration](../resources/workforceintegration.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teamwork/workforceIntegrations
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [workforceIntegration](../resources/workforceintegration.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workforceintegration"
}
-->
``` http
GET https://graph.microsoft.com/localtest/teamwork/workforceIntegrations
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
Content-Length: 1033

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workforceIntegration",
      "id": "2a6dc170-c170-2a6d-70c1-6d2a70c16d2a",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
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
      "supports": "String"
    }
  ]
}
```

