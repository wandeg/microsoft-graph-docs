---
title: "Update tenantSetupInfo"
description: "Update the properties of a tenantSetupInfo object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update tenantSetupInfo
Namespace: microsoft.graph

Update the properties of a [tenantSetupInfo](../resources/tenantsetupinfo.md) object.

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
PATCH /tenantSetupInfo
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [tenantSetupInfo](../resources/tenantsetupinfo.md) object.

The following table shows the properties that are required when you create the [tenantSetupInfo](../resources/tenantsetupinfo.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|userRolesActions|String|**TODO: Add Description**|
|firstTimeSetup|Boolean|**TODO: Add Description**|
|relevantRolesSettings|String collection|**TODO: Add Description**|
|skipSetup|Boolean|**TODO: Add Description**|
|setupStatus|setupStatus|**TODO: Add Description**. Possible values are: `unknown`, `notRegisteredYet`, `registeredSetupNotStarted`, `registeredSetupInProgress`, `registrationAndSetupCompleted`, `registrationFailed`, `registrationTimedOut`, `disabled`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [tenantSetupInfo](../resources/tenantsetupinfo.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_tenantsetupinfo"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/tenantSetupInfo
Content-Type: application/json
Content-length: 227

{
  "@odata.type": "#microsoft.graph.tenantSetupInfo",
  "userRolesActions": "String",
  "firstTimeSetup": "Boolean",
  "relevantRolesSettings": [
    "String"
  ],
  "skipSetup": "Boolean",
  "setupStatus": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.tenantSetupInfo",
  "id": "57dfdcc8-dcc8-57df-c8dc-df57c8dcdf57",
  "userRolesActions": "String",
  "firstTimeSetup": "Boolean",
  "relevantRolesSettings": [
    "String"
  ],
  "skipSetup": "Boolean",
  "setupStatus": "String"
}
```

