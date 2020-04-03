---
title: "Update groupPolicyDefinitionFile"
description: "Update the properties of a groupPolicyDefinitionFile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update groupPolicyDefinitionFile

Namespace: microsoft.graph

Update the properties of a [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) object.

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
PATCH /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) object.

The following table shows the properties that are required when you create the [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|languageCodes|String collection||
|targetPrefix|String||
|targetNamespace|String||
|policyType|Enumeration| Possible values are: `admxBacked`, `admxIngested`.|
|revision|String||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_grouppolicydefinitionfile"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
Content-type: application/json
Content-length: 352

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "String",
  "revision": "Revision value"
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
Content-Length: 465

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "id": "886b3e51-3e51-886b-513e-6b88513e6b88",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "String",
  "revision": "Revision value",
  "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00"
}
```

