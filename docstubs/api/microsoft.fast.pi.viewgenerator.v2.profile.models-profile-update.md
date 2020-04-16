---
title: "Update profile"
description: "Update the properties of a profile object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update profile

Namespace: Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models

Update the properties of a [profile](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-profile.md) object.

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
PATCH /user/{userId}/profile
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [profile](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-profile.md) object.

The following table shows the properties that are required when you create the [profile](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-profile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [profile](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-profile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_profile"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/user/{userId}/profile
Content-Type: application/json
Content-length: 83

{
  "@odata.type": "#Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.profile"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.profile",
  "id": "162abba9-bba9-162a-a9bb-2a16a9bb2a16"
}
```

