---
title: "policySet: getPolicySets"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# getPolicySets

Namespace: microsoft.graph

**TODO: Add Description**

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
POST /deviceAppManagement/policySets/getPolicySets
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|policySetIds|String collection|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [policySet](../resources/policyset.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "policyset_getpolicysets"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/getPolicySets

Content-Type: application/json
Content-length: 44

{
  "policySetIds": [
    "String"
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.policyset)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.policySet",
      "id": "String (identifier)",
      "createdDateTime": "String (timestamp)",
      "lastModifiedDateTime": "String (timestamp)",
      "displayName": "String",
      "description": "String",
      "status": "String",
      "errorCode": "String",
      "guidedDeploymentTags": [
        "String"
      ],
      "roleScopeTags": [
        "String"
      ]
    }
  ]
}
```

