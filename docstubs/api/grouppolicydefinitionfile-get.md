---
title: "Get groupPolicyDefinitionFile"
description: "Read properties and relationships of the groupPolicyDefinitionFile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get groupPolicyDefinitionFile

Namespace: microsoft.graph

Read properties and relationships of the [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) object.

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
GET /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
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
If successful, this method returns a `200 OK` response code and [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_grouppolicydefinitionfile"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupPolicyDefinitionFile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 508

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
    "id": "fc5ef1a0-f1a0-fc5e-a0f1-5efca0f15efc",
    "displayName": "Display Name value",
    "description": "Description value",
    "languageCodes": [
      "Language Codes value"
    ],
    "targetPrefix": "Target Prefix value",
    "targetNamespace": "Target Namespace value",
    "policyType": "String",
    "revision": "Revision value",
    "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00"
  }
}
```

