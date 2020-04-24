---
title: "Create policySets"
description: "Create a new policySets object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create policySets

Namespace: microsoft.graph

Create a new policySets object.

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
POST /deviceAppManagement/policySets
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [policySet](../resources/policyset.md) object.

The following table shows the properties that are required when you create the [policySet](../resources/policyset.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|Creation time of the PolicySet.|
|lastModifiedDateTime|DateTimeOffset|Last modified time of the PolicySet.|
|displayName|String|DisplayName of the PolicySet.|
|description|String|Description of the PolicySet.|
|status|policySetStatus|Validation/assignment status of the PolicySet. Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|errorCode|Error code if any occured. Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|String collection|Tags of the guided deployment|
|roleScopeTags|String collection|RoleScopeTags of the PolicySet|



## Response
If successful, this method returns a `201 Created` response code and a [policySet](../resources/policyset.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_policyset_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets
Content-Type: application/json
Content-length: 307

{
  "@odata.type": "#microsoft.graph.policySet",
  "displayName": "Display Name value",
  "description": "Description value",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "roleScopeTags": [
    "Role Scope Tags value"
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.policyset"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.policySet",
  "id": "b3382f98-2f98-b338-982f-38b3982f38b3",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "roleScopeTags": [
    "Role Scope Tags value"
  ]
}
```

