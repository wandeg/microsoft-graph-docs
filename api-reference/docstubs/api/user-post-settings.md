---
title: "Create settings"
description: "Create a new settings object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create settings

Namespace: microsoft.graph

Create a new settings object.

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
POST /me/settings
POST /users/{usersId}/settings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [userSettings](../resources/usersettings.md) object.

The following table shows the properties that are required when you create the [userSettings](../resources/usersettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|contributionToContentDiscoveryDisabled|Boolean|**TODO: Add Description**|
|contributionToContentDiscoveryAsOrganizationDisabled|Boolean|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [userSettings](../resources/usersettings.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_usersettings_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/settings
Content-Type: application/json
Content-length: 180

{
  "@odata.type": "#microsoft.graph.userSettings",
  "contributionToContentDiscoveryDisabled": "Boolean",
  "contributionToContentDiscoveryAsOrganizationDisabled": "Boolean"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.usersettings"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.userSettings",
  "id": "5fe93de6-3de6-5fe9-e63d-e95fe63de95f",
  "contributionToContentDiscoveryDisabled": "Boolean",
  "contributionToContentDiscoveryAsOrganizationDisabled": "Boolean"
}
```

