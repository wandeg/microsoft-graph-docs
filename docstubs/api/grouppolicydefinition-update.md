---
title: "Update groupPolicyDefinition"
description: "Update the properties of a groupPolicyDefinition object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update groupPolicyDefinition

Namespace: microsoft.graph

Update the properties of a [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.

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
PATCH /deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.

The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/grouppolicydefinition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|classType|Enumeration| Possible values are: `user`, `machine`.|
|displayName|String||
|explainText|String||
|categoryPath|String||
|supportedOn|String||
|policyType|Enumeration| Possible values are: `admxBacked`, `admxIngested`.|
|groupPolicyCategoryId|Guid||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/grouppolicydefinition.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_grouppolicydefinition"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
Content-type: application/json
Content-length: 346

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "String",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "String",
  "groupPolicyCategoryId": "a1303f3a-3f3a-a130-3a3f-30a13a3f30a1"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 459

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "id": "b18ae3e9-e3e9-b18a-e9e3-8ab1e9e38ab1",
  "classType": "String",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "String",
  "groupPolicyCategoryId": "a1303f3a-3f3a-a130-3a3f-30a13a3f30a1",
  "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00"
}
```

