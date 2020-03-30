---
title: "Get auditEvent"
description: "Read properties and relationships of the auditEvent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get auditEvent

Namespace: microsoft.graph

Read properties and relationships of the [auditEvent](../resources/auditevent.md) object.

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
GET /deviceManagement/auditEvents/{auditEventId}
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
If successful, this method returns a `200 OK` response code and [auditEvent](../resources/auditevent.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_auditevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/{auditEventId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.auditEvent"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1590

{
  "value": {
    "@odata.type": "#microsoft.graph.auditEvent",
    "id": "95fb5ad2-5ad2-95fb-d25a-fb95d25afb95",
    "displayName": "Display Name value",
    "componentName": "Component Name value",
    "actor": {
      "@odata.type": "microsoft.graph.auditActor",
      "type": "Type value",
      "userPermissions": [
        "User Permissions value"
      ],
      "applicationId": "Application Id value",
      "applicationDisplayName": "Application Display Name value",
      "userPrincipalName": "User Principal Name value",
      "servicePrincipalName": "Service Principal Name value",
      "ipAddress": "Ip Address value",
      "userId": "User Id value",
      "userRoleScopeTags": [
        {
          "@odata.type": "microsoft.graph.roleScopeTagInfo",
          "roleScopeTagId": "Role Scope Tag Id value"
        }
      ]
    },
    "activity": "Activity value",
    "activityDateTime": "2017-01-01T00:02:05.7806384+03:00",
    "activityType": "Activity Type value",
    "activityOperationType": "Activity Operation Type value",
    "activityResult": "Activity Result value",
    "correlationId": "07153fa5-3fa5-0715-a53f-1507a53f1507",
    "resources": [
      {
        "@odata.type": "microsoft.graph.auditResource",
        "modifiedProperties": [
          {
            "@odata.type": "microsoft.graph.auditProperty",
            "oldValue": "Old Value value",
            "newValue": "New Value value"
          }
        ],
        "resourceId": "Resource Id value"
      }
    ],
    "category": "Category value"
  }
}
```

