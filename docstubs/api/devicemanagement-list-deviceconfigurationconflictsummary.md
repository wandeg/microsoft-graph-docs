---
title: "List deviceConfigurationConflictSummary"
description: "Get the deviceConfigurationConflictSummaries from the deviceConfigurationConflictSummary navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceConfigurationConflictSummary

Namespace: microsoft.graph

Get the deviceConfigurationConflictSummaries from the deviceConfigurationConflictSummary navigation property.

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
GET /deviceManagement/deviceConfigurationConflictSummary
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
If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_deviceconfigurationconflictsummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.deviceconfigurationconflictsummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 495

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
      "id": "b03194f6-94f6-b031-f694-31b0f69431b0",
      "conflictingDeviceConfigurations": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "contributingSettings": [
        "Contributing Settings value"
      ],
      "deviceCheckinsImpacted": 6
    }
  ]
}
```

