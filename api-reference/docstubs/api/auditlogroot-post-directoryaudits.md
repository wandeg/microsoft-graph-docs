---
title: "Create directoryAudits"
description: "Create a new directoryAudits object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create directoryAudits

Namespace: microsoft.graph

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
In the request body, supply a JSON representation of the [directoryAudit](../resources/directoryaudit.md) object.

The following table shows the properties that are required when you create the [directoryAudit](../resources/directoryaudit.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|category|String|**TODO: Add Description**|
|correlationId|String|**TODO: Add Description**|
|result|operationResult|**TODO: Add Description**. Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.|
|resultReason|String|**TODO: Add Description**|
|activityDisplayName|String|**TODO: Add Description**|
|activityDateTime|DateTimeOffset|**TODO: Add Description**|
|loggedByService|String|**TODO: Add Description**|
|operationType|String|**TODO: Add Description**|
|initiatedBy|[auditActivityInitiator](../resources/auditactivityinitiator.md)|**TODO: Add Description**|
|targetResources|[targetResource](../resources/targetresource.md) collection|**TODO: Add Description**|
|additionalDetails|[keyValue](../resources/keyvalue.md) collection|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [directoryAudit](../resources/directoryaudit.md) object in the response body.

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
Content-length: 1484

{
  "@odata.type": "#microsoft.graph.directoryAudit",
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
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryaudit"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
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
```

