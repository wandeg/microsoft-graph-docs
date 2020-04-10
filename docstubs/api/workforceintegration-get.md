---
title: "Get workforceIntegration"
description: "Read properties and relationships of the workforceIntegration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get workforceIntegration

Namespace: microsoft.graph

Read properties and relationships of the [workforceIntegration](../resources/workforceintegration.md) object.

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
GET /teamwork/workforceIntegrations/{workforceIntegrationId}
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
If successful, this method returns a `200 OK` response code and [workforceIntegration](../resources/workforceintegration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_workforceintegration"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/workforceIntegrations/{workforceIntegrationId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1000

{
  "value": {
    "@odata.type": "#microsoft.graph.workforceIntegration",
    "id": "adc60d46-0d46-adc6-460d-c6ad460dc6ad",
    "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
    "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
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
}
```

