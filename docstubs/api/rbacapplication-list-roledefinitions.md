---
title: "List roleDefinitions"
description: "Get the unifiedRoleDefinitions from the roleDefinitions navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List roleDefinitions

Namespace: microsoft.graph

Get the unifiedRoleDefinitions from the roleDefinitions navigation property.

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
GET /roleManagement/directory/roleDefinitions
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
If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_unifiedroledefinition"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.unifiedroledefinition)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 808

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.unifiedRoleDefinition",
      "id": "8872b1de-b1de-8872-deb1-7288deb17288",
      "description": "Description value",
      "displayName": "Display Name value",
      "isBuiltIn": true,
      "isEnabled": true,
      "resourceScopes": [
        "Resource Scopes value"
      ],
      "rolePermissions": [
        {
          "@odata.type": "microsoft.graph.unifiedRolePermission",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "excludedResourceActions": [
            "Excluded Resource Actions value"
          ],
          "condition": "Condition value"
        }
      ],
      "templateId": "Template Id value",
      "version": "Version value"
    }
  ]
}
```

