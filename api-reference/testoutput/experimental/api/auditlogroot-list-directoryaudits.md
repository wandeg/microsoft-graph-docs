---
title: "List directoryAudits"
description: "Get the directoryAudits from the directoryAudits navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List directoryAudits

Namespace: microsoft.graph

Get the directoryAudits from the directoryAudits navigation property.

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
GET /auditLogs/directoryAudits
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [directoryAudit](../resources/directoryaudit.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_directoryaudit"
}
-->
``` http
GET https://graph.microsoft.com/localtest/auditLogs/directoryAudits
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.directoryaudit)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1754

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.directoryAudit",
      "id": "c8d329d5-29d5-c8d3-d529-d3c8d529d3c8",
      "category": "Category value",
      "correlationId": "Correlation Id value",
      "result": "String",
      "resultReason": "Result Reason value",
      "activityDisplayName": "Activity Display Name value",
      "activityDateTime": "2016-12-31T23:57:38.3073089+03:00",
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
  ]
}
```

