---
title: "Get groupPolicyDefinition"
description: "Read properties and relationships of the groupPolicyDefinition object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get groupPolicyDefinition

Namespace: microsoft.graph

Read properties and relationships of the [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.

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
GET /deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
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
If successful, this method returns a `200 OK` response code and [groupPolicyDefinition](../resources/grouppolicydefinition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_grouppolicydefinition"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupPolicyDefinition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 498

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyDefinition",
    "id": "bcc89f77-9f77-bcc8-779f-c8bc779fc8bc",
    "classType": "String",
    "displayName": "Display Name value",
    "explainText": "Explain Text value",
    "categoryPath": "Category Path value",
    "supportedOn": "Supported On value",
    "policyType": "String",
    "groupPolicyCategoryId": "b3541151-1151-b354-5111-54b3511154b3",
    "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00"
  }
}
```

