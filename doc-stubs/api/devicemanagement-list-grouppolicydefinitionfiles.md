---
title: "List groupPolicyDefinitionFiles"
description: "Get the groupPolicyDefinitionFiles from the groupPolicyDefinitionFiles navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List groupPolicyDefinitionFiles

Namespace: microsoft.graph

Get the groupPolicyDefinitionFiles from the groupPolicyDefinitionFiles navigation property.

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
GET /deviceManagement/groupPolicyDefinitionFiles
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

If successful, this method returns a `200 OK` response code and a collection of [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_grouppolicydefinitionfile"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitionFiles
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.grouppolicydefinitionfile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
      "id": "a398fe80-fe80-a398-80fe-98a380fe98a3",
      "displayName": "String",
      "description": "String",
      "languageCodes": [
        "String"
      ],
      "targetPrefix": "String",
      "targetNamespace": "String",
      "policyType": "String",
      "revision": "String",
      "lastModifiedDateTime": "String (timestamp)"
    }
  ]
}
```

