---
title: "Create directoryAudits"
description: "Create a new directoryAudits object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create directoryAudits

Namespace: Microsoft.AAD.Reporting

Create a new directoryAudits object.

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
POST /auditLogs/directoryAudits
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [directoryAudit](../resources/microsoft.aad.reporting-directoryaudit.md) object.

The following table shows the properties that are required when you create the [directoryAudit](../resources/microsoft.aad.reporting-directoryaudit.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|category|String|**TODO: Add Description**|
|correlationId|String|**TODO: Add Description**|
|result|operationResult|**TODO: Add Description**. Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.|
|resultReason|String|**TODO: Add Description**|
|activityDisplayName|String|**TODO: Add Description**|
|activityDateTime|DateTimeOffset|**TODO: Add Description**|
|loggedByService|String|**TODO: Add Description**|
|operationType|String|**TODO: Add Description**|
|initiatedBy|[auditActivityInitiator](../resources/microsoft.aad.reporting-auditactivityinitiator.md)|**TODO: Add Description**|
|targetResources|[targetResource](../resources/microsoft.aad.reporting-targetresource.md) collection|**TODO: Add Description**|
|additionalDetails|[keyValue](../resources/microsoft.aad.reporting-keyvalue.md) collection|**TODO: Add Description**|



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
Content-Type: application/json
Content-length: 1540

{
  "@odata.type": "#Microsoft.AAD.Reporting.directoryAudit",
  "category": "Category value",
  "correlationId": "Correlation Id value",
  "result": "String",
  "resultReason": "Result Reason value",
  "activityDisplayName": "Activity Display Name value",
  "activityDateTime": "2017-01-01T00:03:11.0875532+00:00",
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
{
  "@odata.type": "#Microsoft.AAD.Reporting.directoryAudit",
  "id": "44edbe4f-be4f-44ed-4fbe-ed444fbeed44",
  "category": "Category value",
  "correlationId": "Correlation Id value",
  "result": "String",
  "resultReason": "Result Reason value",
  "activityDisplayName": "Activity Display Name value",
  "activityDateTime": "2017-01-01T00:03:11.0875532+00:00",
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

