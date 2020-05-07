---
title: "Create teamsApps"
description: "Create a new teamsApps object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create teamsApps

Namespace: microsoft.graph

Create a new teamsApps object.

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
POST /appCatalogs/teamsApps
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [teamsApp](../resources/teamsapp.md) object.

The following table shows the properties that are required when you create the [teamsApp](../resources/teamsapp.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|externalId|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|distributionMethod|teamsAppDistributionMethod|**TODO: Add Description**. Possible values are: `store`, `organization`, `sideloaded`, `unknownFutureValue`.|



## Response

If successful, this method returns a `201 Created` response code and a [teamsApp](../resources/teamsapp.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_teamsapp_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-Type: application/json
Content-length: 161

{
  "@odata.type": "#microsoft.graph.teamsApp",
  "externalId": "String",
  "name": "String",
  "displayName": "String",
  "distributionMethod": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsapp"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.teamsApp",
  "id": "19261bd7-1bd7-1926-d71b-2619d71b2619",
  "externalId": "String",
  "name": "String",
  "displayName": "String",
  "distributionMethod": "String"
}
```

