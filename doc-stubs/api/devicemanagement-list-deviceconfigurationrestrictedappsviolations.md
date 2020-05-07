---
title: "List deviceConfigurationRestrictedAppsViolations"
description: "Get the restrictedAppsViolations from the deviceConfigurationRestrictedAppsViolations navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List deviceConfigurationRestrictedAppsViolations

Namespace: microsoft.graph

Get the restrictedAppsViolations from the deviceConfigurationRestrictedAppsViolations navigation property.

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
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations
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

If successful, this method returns a `200 OK` response code and a collection of [restrictedAppsViolation](../resources/restrictedappsviolation.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_restrictedappsviolation"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.restrictedappsviolation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.restrictedAppsViolation",
      "id": "3060e475-e475-3060-75e4-603075e46030",
      "userId": "String",
      "userName": "String",
      "managedDeviceId": "String",
      "deviceName": "String",
      "deviceConfigurationId": "String",
      "deviceConfigurationName": "String",
      "platformType": "String",
      "restrictedAppsState": "String",
      "restrictedApps": [
        {
          "@odata.type": "microsoft.graph.managedDeviceReportedApp"
        }
      ]
    }
  ]
}
```

