---
title: "Add policySets"
description: "Add policySets by posting to the policySets collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add policySets

Namespace: microsoft.graph

Add policySets by posting to the policySets collection.

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
POST /deviceAppManagement/policySets/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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

## Examples

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
Content-Length: 479

{
  "@odata.type": "#microsoft.graph.policySet",
  "id": "b9715cea-5cea-b971-ea5c-71b9ea5c71b9",
  "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
  "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00",
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

