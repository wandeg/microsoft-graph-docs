---
title: "List securityBaselineCategoryStateSummaries"
description: "List properties and relationships of the securityBaselineCategoryStateSummary objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List securityBaselineCategoryStateSummaries

Namespace: microsoft.graph

List properties and relationships of the [securityBaselineCategoryStateSummary](../resources/securitybaselinecategorystatesummary.md) objects.

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
GET /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [securityBaselineCategoryStateSummary](../resources/securitybaselinecategorystatesummary.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_securitybaselinecategorystatesummary"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.securitybaselinecategorystatesummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 379

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
      "id": "4a601bdb-1bdb-4a60-db1b-604adb1b604a",
      "secureCount": 11,
      "notSecureCount": 14,
      "unknownCount": 12,
      "errorCount": 10,
      "conflictCount": 13,
      "notApplicableCount": 2,
      "displayName": "Display Name value"
    }
  ]
}
```

