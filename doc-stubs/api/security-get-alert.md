---
title: "Get alerts"
description: "Read the properties and relationships of an alert object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get alerts

Namespace: microsoft.graph

Read the properties and relationships of an [alert](../resources/alert.md) object.

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
GET /Security/alerts
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [alert](../resources/alert.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_alert"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/Security/alerts
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.alert",
    "id": "bc644f3a-4f3a-bc64-3a4f-64bc3a4f64bc",
    "activityGroupName": "String",
    "assignedTo": "String",
    "azureSubscriptionId": "String",
    "azureTenantId": "String",
    "category": "String",
    "closedDateTime": "String (timestamp)",
    "cloudAppStates": [
      {
        "@odata.type": "microsoft.graph.cloudAppSecurityState"
      }
    ],
    "comments": [
      "String"
    ],
    "confidence": "Integer",
    "createdDateTime": "String (timestamp)",
    "description": "String",
    "detectionIds": [
      "String"
    ],
    "eventDateTime": "String (timestamp)",
    "feedback": "String",
    "fileStates": [
      {
        "@odata.type": "microsoft.graph.fileSecurityState"
      }
    ],
    "historyStates": [
      {
        "@odata.type": "microsoft.graph.alertHistoryState"
      }
    ],
    "hostStates": [
      {
        "@odata.type": "microsoft.graph.hostSecurityState"
      }
    ],
    "lastModifiedDateTime": "String (timestamp)",
    "malwareStates": [
      {
        "@odata.type": "microsoft.graph.malwareState"
      }
    ],
    "networkConnections": [
      {
        "@odata.type": "microsoft.graph.networkConnection"
      }
    ],
    "processes": [
      {
        "@odata.type": "microsoft.graph.process"
      }
    ],
    "recommendedActions": [
      "String"
    ],
    "registryKeyStates": [
      {
        "@odata.type": "microsoft.graph.registryKeyState"
      }
    ],
    "severity": "String",
    "sourceMaterials": [
      "String"
    ],
    "status": "String",
    "tags": [
      "String"
    ],
    "title": "String",
    "triggers": [
      {
        "@odata.type": "microsoft.graph.alertTrigger"
      }
    ],
    "userStates": [
      {
        "@odata.type": "microsoft.graph.userSecurityState"
      }
    ],
    "vendorInformation": {
      "@odata.type": "microsoft.graph.securityVendorInformation"
    },
    "vulnerabilityStates": [
      {
        "@odata.type": "microsoft.graph.vulnerabilityState"
      }
    ]
  }
}
```

