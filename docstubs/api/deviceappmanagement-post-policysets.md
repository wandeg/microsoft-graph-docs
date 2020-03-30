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
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [policySet](../resources/policyset.md) object.

The following table shows the properties that are required when you create the [policySet](../resources/policyset.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset||
|lastModifiedDateTime|DateTimeOffset||
|displayName|String||
|description|String||
|status|Enumeration| Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|Enumeration| Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|String collection||
|roleScopeTags|String collection||



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
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets
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
  "id": "13a71be9-1be9-13a7-e91b-a713e91ba713",
  "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
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

