---
title: "Create profile"
description: "Create a new profile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create profile

Namespace: microsoft.graph

Create a new profile object.

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
POST /user/{userId}/profile
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [profile](../resources/profile.md) object.

The following table shows the properties that are required when you create the [profile](../resources/profile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [profile](../resources/profile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_profile_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/user/{userId}/profile
Content-Type: application/json
Content-length: 83

{
  "@odata.type": "#Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.profile"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.fast.pi.viewgenerator.v2.profile.models.profile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.profile",
  "id": "1736e66d-e66d-1736-6de6-36176de63617"
}
```

