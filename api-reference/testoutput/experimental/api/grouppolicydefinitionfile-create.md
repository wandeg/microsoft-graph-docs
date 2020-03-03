---
title: "Create groupPolicyDefinitionFile"
description: "Create a new groupPolicyDefinitionFile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create groupPolicyDefinitionFile

Namespace: microsoft.graph

Create a new [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) object.

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
POST /deviceManagement/groupPolicyDefinitionFiles
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) object.

The following table shows the properties that are required when you create the [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|The localized friendly name of the ADMX file.|
|description|String|The localized description of the policy settings in the ADMX file. The default value is empty.|
|languageCodes|String collection|The supported language codes for the ADMX file.|
|targetPrefix|String|Specifies the logical name that refers to the namespace within the ADMX file.|
|targetNamespace|String|Specifies the URI used to identify the namespace within the ADMX file.|
|policyType|Enumeration|Specifies the type of group policy. Possible values are: `admxBacked`, `admxIngested`.|
|revision|String|The revision version associated with the file.|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified.|



## Response
If successful, this method returns a `201 Created` response code and a [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_grouppolicydefinitionfile_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/groupPolicyDefinitionFiles
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
  "truncated": true,
  "@odata.type": "microsoft.graph.grouppolicydefinitionfile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 465

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "id": "d7ab3a02-3a02-d7ab-023a-abd7023aabd7",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "String",
  "revision": "Revision value",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00"
}
```

