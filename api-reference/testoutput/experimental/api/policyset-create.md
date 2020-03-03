---
title: "Create policySet"
description: "Create a new policySet object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create policySet

Namespace: microsoft.graph

Create a new [policySet](../resources/policyset.md) object.

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
POST /deviceAppManagement/policySets
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [policySet](../resources/policyset.md) object.

The following table shows the properties that are required when you create the [policySet](../resources/policyset.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|Creation time of the PolicySet.|
|lastModifiedDateTime|DateTimeOffset|Last modified time of the PolicySet.|
|displayName|String|DisplayName of the PolicySet.|
|description|String|Description of the PolicySet.|
|status|Enumeration|Validation/assignment status of the PolicySet. Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|Enumeration|Error code if any occured. Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|String collection|Tags of the guided deployment|
|roleScopeTags|String collection|RoleScopeTags of the PolicySet|



## Response
If successful, this method returns a `201 Created` response code and a [policySet](../resources/policyset.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_policyset_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceAppManagement/policySets
Content-type: application/json
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.policyset"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 478

{
  "@odata.type": "#microsoft.graph.policySet",
  "id": "69cb9a4c-9a4c-69cb-4c9a-cb694c9acb69",
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
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

