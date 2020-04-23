---
title: "Get directoryAudit"
description: "Read the properties and relationships of a directoryAudit object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get directoryAudit

Namespace: microsoft.graph

Read the properties and relationships of a [directoryAudit](../resources/directoryaudit.md) object.

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
GET /auditLogs/directoryAudits/{directoryAuditId}
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
If successful, this method returns a `200 OK` response code and a [directoryAudit](../resources/directoryaudit.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_directoryaudit"
}
-->
``` http
GET https://graph.microsoft.com/beta/auditLogs/directoryAudits/{directoryAuditId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryAudit"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.directoryAudit",
    "id": "027b1cf2-1cf2-027b-f21c-7b02f21c7b02",
    "category": "Category value",
    "correlationId": "Correlation Id value",
    "result": "String",
    "resultReason": "Result Reason value",
    "activityDisplayName": "Activity Display Name value",
    "activityDateTime": "2016-12-31T23:56:30.5894076+03:00",
    "loggedByService": "Logged By Service value",
    "operationType": "Operation Type value",
    "initiatedBy": {
      "@odata.type": "microsoft.graph.auditActivityInitiator",
      "user": {
        "@odata.type": "microsoft.graph.userIdentity",
        "id": "Id value",
        "displayName": "Display Name value",
        "ipAddress": "Ip Address value",
        "userPrincipalName": "User Principal Name value"
      },
      "app": {
        "@odata.type": "microsoft.graph.appIdentity",
        "appId": "App Id value",
        "servicePrincipalId": "Service Principal Id value",
        "servicePrincipalName": "Service Principal Name value"
      }
    },
    "targetResources": [
      {
        "@odata.type": "microsoft.graph.targetResource",
        "type": "Type value",
        "groupType": "String",
        "modifiedProperties": [
          {
            "@odata.type": "microsoft.graph.modifiedProperty",
            "oldValue": "Old Value value",
            "newValue": "New Value value"
          }
        ]
      }
    ],
    "additionalDetails": [
      {
        "@odata.type": "microsoft.graph.keyValue",
        "key": "Key value",
        "value": "Value value"
      }
    ]
  }
}
```

