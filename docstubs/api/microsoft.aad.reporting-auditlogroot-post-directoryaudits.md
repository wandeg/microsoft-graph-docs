---
title: "Add directoryAudits"
description: "Add directoryAudits by posting to the directoryAudits collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add directoryAudits

Namespace: Microsoft.AAD.Reporting

Add directoryAudits by posting to the directoryAudits collection.

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
POST /auditLogs/directoryAudits/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [directoryAudit](../resources/microsoft.aad.reporting-directoryaudit.md) object.

The following table shows the properties that are required when you create the [directoryAudit](../resources/microsoft.aad.reporting-directoryaudit.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String||
|category|String||
|correlationId|String||
|result|Enumeration| Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.|
|resultReason|String||
|activityDisplayName|String||
|activityDateTime|DateTimeOffset||
|loggedByService|String||
|operationType|String||
|initiatedBy|[auditActivityInitiator](../resources/microsoft.aad.reporting-auditactivityinitiator.md)||
|targetResources|[targetResource](../resources/microsoft.aad.reporting-targetresource.md) collection||
|additionalDetails|[keyValue](../resources/microsoft.aad.reporting-keyvalue.md) collection||



## Response
If successful, this method returns a `201 Created` response code and a [directoryAudit](../resources/microsoft.aad.reporting-directoryaudit.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_directoryaudit_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/auditLogs/directoryAudits
Content-type: application/json
Content-length: 1540

{
  "@odata.type": "#Microsoft.AAD.Reporting.directoryAudit",
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
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.aad.reporting.directoryaudit"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1589

{
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
```

