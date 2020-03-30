---
title: "Add auditEvents"
description: "Add auditEvents by posting to the auditEvents collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add auditEvents

Namespace: microsoft.graph

Add auditEvents by posting to the auditEvents collection.

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
POST /deviceManagement/auditEvents/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [auditEvent](../resources/auditevent.md) object.

The following table shows the properties that are required when you create the [auditEvent](../resources/auditevent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|componentName|String||
|actor|[auditActor](../resources/auditactor.md)||
|activity|String||
|activityDateTime|DateTimeOffset||
|activityType|String||
|activityOperationType|String||
|activityResult|String||
|correlationId|Guid||
|resources|[auditResource](../resources/auditresource.md) collection||
|category|String||



## Response
If successful, this method returns a `201 Created` response code and a [auditEvent](../resources/auditevent.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_auditevent_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/auditEvents
Content-type: application/json
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
  "activityDateTime": "2017-01-01T00:01:53.7837706+03:00",
  "activityType": "Activity Type value",
  "activityOperationType": "Activity Operation Type value",
  "activityResult": "Activity Result value",
  "correlationId": "95185d57-5d57-9518-575d-1895575d1895",
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.auditevent"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1485

{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "c57e957b-957b-c57e-7b95-7ec57b957ec5",
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
  "activityDateTime": "2017-01-01T00:01:53.7837706+03:00",
  "activityType": "Activity Type value",
  "activityOperationType": "Activity Operation Type value",
  "activityResult": "Activity Result value",
  "correlationId": "95185d57-5d57-9518-575d-1895575d1895",
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

