---
title: "privilegedSignupStatus: completeSetup"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# completeSetup

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
POST /privilegedSignupStatus/completeSetup
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
|tenantSetupInfo|[tenantSetupInfo](../resources/tenantsetupinfo.md)|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [roleSuccessStatistics](../resources/rolesuccessstatistics.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "privilegedsignupstatus_completesetup"
}
-->
``` http
POST https://graph.microsoft.com/beta/privilegedSignupStatus/completeSetup

Content-Type: application/json
Content-length: 306

{
  "tenantSetupInfo": {
    "@odata.type": "#microsoft.graph.tenantSetupInfo",
    "id": "String (identifier)",
    "userRolesActions": "String",
    "firstTimeSetup": "Boolean",
    "relevantRolesSettings": [
      "String"
    ],
    "skipSetup": "Boolean",
    "setupStatus": "String"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.rolesuccessstatistics)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "microsoft.graph.roleSuccessStatistics"
    }
  ]
}
```

