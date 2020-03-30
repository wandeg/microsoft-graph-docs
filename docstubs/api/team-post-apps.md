---
title: "Add apps"
description: "Add apps by posting to the apps collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add apps

Namespace: microsoft.graph

Add apps by posting to the apps collection.

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
POST /teams/{teamsId}/apps/$ref
POST /me/joinedGroups/{groupId}/team/apps/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [teamsCatalogApp](../resources/teamscatalogapp.md) object.

The following table shows the properties that are required when you create the [teamsCatalogApp](../resources/teamscatalogapp.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|externalId|String||
|name|String||
|distributionMethod|Enumeration| Possible values are: `store`, `organization`, `sideloaded`, `unknownFutureValue`.|



## Response
If successful, this method returns a `201 Created` response code and a [teamsCatalogApp](../resources/teamscatalogapp.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_teamscatalogapp_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamsId}/apps
Content-type: application/json
Content-length: 155

{
  "@odata.type": "#microsoft.graph.teamsCatalogApp",
  "externalId": "External Id value",
  "name": "Name value",
  "distributionMethod": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamscatalogapp"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 204

{
  "@odata.type": "#microsoft.graph.teamsCatalogApp",
  "id": "e220e41b-e41b-e220-1be4-20e21be420e2",
  "externalId": "External Id value",
  "name": "Name value",
  "distributionMethod": "String"
}
```

