---
title: "Get directoryAudit"
description: "Read properties and relationships of the directoryAudit object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get directoryAudit

Namespace: Microsoft.AAD.Reporting

Read properties and relationships of the [directoryAudit](../resources/microsoft.aad.reporting-directoryaudit.md) object.

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
GET /auditLogs/directoryAudits/{directoryAuditId}
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
If successful, this method returns a `200 OK` response code and [directoryAudit](../resources/microsoft.aad.reporting-directoryaudit.md) object in the response body.

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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.AAD.Reporting.directoryAudit"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1702

{
  "value": {
    "@odata.type": "#Microsoft.AAD.Reporting.directoryAudit",
    "id": "3a89a4c2-a4c2-3a89-c2a4-893ac2a4893a",
    "category": "Category value",
    "correlationId": "Correlation Id value",
    "result": "String",
    "resultReason": "Result Reason value",
    "activityDisplayName": "Activity Display Name value",
    "activityDateTime": "2016-12-31T23:56:54.8488209+00:00",
    "loggedByService": "Logged By Service value",
    "operationType": "Operation Type value",
    "initiatedBy": {
      "@odata.type": "Microsoft.AAD.Reporting.auditActivityInitiator",
      "user": {
        "@odata.type": "Microsoft.AAD.Reporting.userIdentity",
        "id": "Id value",
        "displayName": "Display Name value",
        "ipAddress": "Ip Address value",
        "userPrincipalName": "User Principal Name value"
      },
      "app": {
        "@odata.type": "Microsoft.AAD.Reporting.appIdentity",
        "appId": "App Id value",
        "servicePrincipalId": "Service Principal Id value",
        "servicePrincipalName": "Service Principal Name value"
      }
    },
    "targetResources": [
      {
        "@odata.type": "Microsoft.AAD.Reporting.targetResource",
        "type": "Type value",
        "groupType": "String",
        "modifiedProperties": [
          {
            "@odata.type": "Microsoft.AAD.Reporting.modifiedProperty",
            "oldValue": "Old Value value",
            "newValue": "New Value value"
          }
        ]
      }
    ],
    "additionalDetails": [
      {
        "@odata.type": "Microsoft.AAD.Reporting.keyValue",
        "key": "Key value",
        "value": "Value value"
      }
    ]
  }
}
```

