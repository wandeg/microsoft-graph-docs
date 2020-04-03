---
title: "Create definitions"
description: "Create definitions by posting to the definitions collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create definitions

Namespace: microsoft.graph

Create definitions by posting to the definitions collection.

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
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [groupPolicyDefinition](../resources/grouppolicydefinition.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_grouppolicydefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions
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
  "groupPolicyCategoryId": "944d8837-8837-944d-3788-4d9437884d94"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.grouppolicydefinition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 459

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "id": "58bba6bd-a6bd-58bb-bda6-bb58bda6bb58",
  "classType": "String",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "String",
  "groupPolicyCategoryId": "944d8837-8837-944d-3788-4d9437884d94",
  "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00"
}
```

