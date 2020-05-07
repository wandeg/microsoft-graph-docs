---
title: "List healthStates"
description: "Get the windowsManagementAppHealthStates from the healthStates navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List healthStates

Namespace: microsoft.graph

Get the windowsManagementAppHealthStates from the healthStates navigation property.

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
GET /deviceAppManagement/windowsManagementApp/healthStates
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

If successful, this method returns a `200 OK` response code and a collection of [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_windowsmanagementapphealthstate"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.windowsmanagementapphealthstate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
      "id": "301cf452-f452-301c-52f4-1c3052f41c30",
      "healthState": "String",
      "installedVersion": "String",
      "lastCheckInDateTime": "String (timestamp)",
      "deviceName": "String",
      "deviceOSVersion": "String"
    }
  ]
}
```

