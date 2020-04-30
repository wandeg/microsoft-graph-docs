---
title: "Update apps"
description: "Update the properties of an apps object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update apps

Namespace: microsoft.graph

Update the properties of an apps object.

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
PATCH /teams/{teamsId}/apps
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [teamsCatalogApp](../resources/teamscatalogapp.md) object.

The following table shows the properties that are required when you create the [teamsCatalogApp](../resources/teamscatalogapp.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|externalId|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|distributionMethod|teamsAppDistributionMethod|**TODO: Add Description**. Possible values are: `store`, `organization`, `sideloaded`, `unknownFutureValue`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [teamsCatalogApp](../resources/teamscatalogapp.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_apps"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/teams/{teamsId}/apps
Content-Type: application/json
Content-length: 140

{
  "@odata.type": "#microsoft.graph.teamsCatalogApp",
  "externalId": "String",
  "name": "String",
  "distributionMethod": "String"
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
  "@odata.type": "#microsoft.graph.teamsCatalogApp",
  "id": "969bb333-b333-969b-33b3-9b9633b39b96",
  "externalId": "String",
  "name": "String",
  "distributionMethod": "String"
}
```

