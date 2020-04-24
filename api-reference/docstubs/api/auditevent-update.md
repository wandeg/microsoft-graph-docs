---
title: "Update auditEvent"
description: "Update the properties of an auditEvent object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update auditEvent

Namespace: microsoft.graph

Update the properties of an [auditEvent](../resources/auditevent.md) object.

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
PATCH /deviceManagement/auditEvents/{auditEventId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [auditEvent](../resources/auditevent.md) object.

The following table shows the properties that are required when you create the [auditEvent](../resources/auditevent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|Event display name.|
|componentName|String|Component name.|
|actor|[auditActor](../resources/auditactor.md)|AAD user and application that are associated with the audit event.|
|activity|String|Friendly name of the activity.|
|activityDateTime|DateTimeOffset|The date time in UTC when the activity was performed.|
|activityType|String|The type of activity that was being performed.|
|activityOperationType|String|The HTTP operation type of the activity.|
|activityResult|String|The result of the activity.|
|correlationId|Guid|The client request Id that is used to correlate activity within the system.|
|resources|[auditResource](../resources/auditresource.md) collection|Resources being modified.|
|category|String|Audit category.|



## Response
If successful, this method returns a `200 OK` response code and an updated [auditEvent](../resources/auditevent.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_auditevent"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/auditEvents/{auditEventId}
Content-Type: application/json
Content-length: 1436

{
  "@odata.type": "#microsoft.graph.auditEvent",
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
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
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
```

