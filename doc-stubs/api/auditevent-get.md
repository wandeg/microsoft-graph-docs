---
title: "Get auditEvent"
description: "Read the properties and relationships of an auditEvent object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get auditEvent

Namespace: microsoft.graph

Read the properties and relationships of an [auditEvent](../resources/auditevent.md) object.

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
GET /deviceManagement/auditEvents/{auditEventId}
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

If successful, this method returns a `200 OK` response code and an [auditEvent](../resources/auditevent.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_auditevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/{auditEventId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.auditEvent"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.auditEvent",
    "id": "a4e59548-9548-a4e5-4895-e5a44895e5a4",
    "displayName": "String",
    "componentName": "String",
    "actor": {
      "@odata.type": "microsoft.graph.auditActor"
    },
    "activity": "String",
    "activityDateTime": "String (timestamp)",
    "activityType": "String",
    "activityOperationType": "String",
    "activityResult": "String",
    "correlationId": "Guid",
    "resources": [
      {
        "@odata.type": "microsoft.graph.auditResource"
      }
    ],
    "category": "String"
  }
}
```

