---
title: "updateAlerts"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# updateAlerts

Namespace: microsoft.graph



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
POST /Security/alerts/updateAlerts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|value|[alert](../resources/alert.md) collection||



## Response
If successful, this action returns a `200 OK` response code and a [alert](../resources/alert.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "alert_updatealerts"
}
-->
``` http
POST https://graph.microsoft.com/beta/Security/alerts/updateAlerts

Content-type: application/json
Content-length: 2553

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.alert",
      "id": "711c4cba-4cba-711c-ba4c-1c71ba4c1c71",
      "activityGroupName": "Activity Group Name value",
      "assignedTo": "Assigned To value",
      "azureSubscriptionId": "Azure Subscription Id value",
      "azureTenantId": "Azure Tenant Id value",
      "category": "Category value",
      "closedDateTime": "2017-01-01T00:00:28.7472942+03:00",
      "cloudAppStates": [
        {
          "@odata.type": "microsoft.graph.cloudAppSecurityState"
        }
      ],
      "comments": [
        "Comments value"
      ],
      "confidence": 10,
      "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
      "description": "Description value",
      "detectionIds": [
        "Detection Ids value"
      ],
      "eventDateTime": "2017-01-01T00:02:22.1549518+03:00",
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
      "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
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
        "Recommended Actions value"
      ],
      "registryKeyStates": [
        {
          "@odata.type": "microsoft.graph.registryKeyState"
        }
      ],
      "severity": "String",
      "sourceMaterials": [
        "Source Materials value"
      ],
      "status": "String",
      "tags": [
        "Tags value"
      ],
      "title": "Title value",
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
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.alert)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2553

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.alert",
      "id": "711c4cba-4cba-711c-ba4c-1c71ba4c1c71",
      "activityGroupName": "Activity Group Name value",
      "assignedTo": "Assigned To value",
      "azureSubscriptionId": "Azure Subscription Id value",
      "azureTenantId": "Azure Tenant Id value",
      "category": "Category value",
      "closedDateTime": "2017-01-01T00:00:28.7472942+03:00",
      "cloudAppStates": [
        {
          "@odata.type": "microsoft.graph.cloudAppSecurityState"
        }
      ],
      "comments": [
        "Comments value"
      ],
      "confidence": 10,
      "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
      "description": "Description value",
      "detectionIds": [
        "Detection Ids value"
      ],
      "eventDateTime": "2017-01-01T00:02:22.1549518+03:00",
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
      "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
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
        "Recommended Actions value"
      ],
      "registryKeyStates": [
        {
          "@odata.type": "microsoft.graph.registryKeyState"
        }
      ],
      "severity": "String",
      "sourceMaterials": [
        "Source Materials value"
      ],
      "status": "String",
      "tags": [
        "Tags value"
      ],
      "title": "Title value",
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
  ]
}
```

