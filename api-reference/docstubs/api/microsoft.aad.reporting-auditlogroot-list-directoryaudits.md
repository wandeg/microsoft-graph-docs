---
title: "List directoryAudits"
description: "Get the directoryAudits from the directoryAudits navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List directoryAudits

Namespace: Microsoft.AAD.Reporting

Get the directoryAudits from the directoryAudits navigation property.

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
GET /auditLogs/directoryAudits
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
If successful, this method returns a `200 OK` response code and a collection of [directoryAudit](../resources/directoryaudit.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_directoryaudit"
}
-->
``` http
GET https://graph.microsoft.com/beta/auditLogs/directoryAudits
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.aad.reporting.directoryaudit)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#Microsoft.AAD.Reporting.directoryAudit",
      "id": "ad92015a-015a-ad92-5a01-92ad5a0192ad",
      "category": "Category value",
      "correlationId": "Correlation Id value",
      "result": "String",
      "resultReason": "Result Reason value",
      "activityDisplayName": "Activity Display Name value",
      "activityDateTime": "2017-01-01T00:01:43.992962+03:00",
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
  ]
}
```

