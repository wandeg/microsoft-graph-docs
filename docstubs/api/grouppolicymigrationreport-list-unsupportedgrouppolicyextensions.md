---
title: "List unsupportedGroupPolicyExtensions"
description: "Get the unsupportedGroupPolicyExtensions from the unsupportedGroupPolicyExtensions navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List unsupportedGroupPolicyExtensions

Namespace: microsoft.graph

Get the unsupportedGroupPolicyExtensions from the unsupportedGroupPolicyExtensions navigation property.

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
GET /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
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
If successful, this method returns a `200 OK` response code and a collection of [unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_unsupportedgrouppolicyextension"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.unsupportedgrouppolicyextension)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 342

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.unsupportedGroupPolicyExtension",
      "id": "18b2d3d7-d3d7-18b2-d7d3-b218d7d3b218",
      "settingScope": "String",
      "namespaceUrl": "https://example.com/namespaceUrl/",
      "extensionType": "Extension Type value",
      "nodeName": "Node Name value"
    }
  ]
}
```

