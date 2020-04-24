---
title: "List auditEvents"
description: "Get the auditEvents from the auditEvents navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List auditEvents

Namespace: microsoft.graph

Get the auditEvents from the auditEvents navigation property.

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
GET /deviceManagement/auditEvents
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
If successful, this method returns a `200 OK` response code and a collection of [auditEvent](../resources/auditevent.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_auditevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.auditevent)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.auditEvent",
      "id": "2ce64df9-4df9-2ce6-f94d-e62cf94de62c",
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
      "activityDateTime": "2017-01-01T00:03:07.3452024+03:00",
      "activityType": "Activity Type value",
      "activityOperationType": "Activity Operation Type value",
      "activityResult": "Activity Result value",
      "correlationId": "e32ad00d-d00d-e32a-0dd0-2ae30dd02ae3",
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
  ]
}
```

