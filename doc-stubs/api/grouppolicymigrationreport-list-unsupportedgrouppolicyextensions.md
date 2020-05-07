---
title: "List unsupportedGroupPolicyExtensions"
description: "Get the unsupportedGroupPolicyExtensions from the unsupportedGroupPolicyExtensions navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List unsupportedGroupPolicyExtensions

Namespace: microsoft.graph

Get the unsupportedGroupPolicyExtensions from the unsupportedGroupPolicyExtensions navigation property.

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
GET /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.unsupportedgrouppolicyextension)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.unsupportedGroupPolicyExtension",
      "id": "dfe4bd34-bd34-dfe4-34bd-e4df34bde4df",
      "settingScope": "String",
      "namespaceUrl": "String",
      "extensionType": "String",
      "nodeName": "String"
    }
  ]
}
```

