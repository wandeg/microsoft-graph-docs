---
title: "Create publishedResources"
description: "Create a new publishedResources object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create publishedResources

Namespace: microsoft.graph

Create a new publishedResources object.

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
POST /onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}/publishedResources
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [publishedResource](../resources/publishedresource.md) object.

The following table shows the properties that are required when you create the [publishedResource](../resources/publishedresource.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|resourceName|String|**TODO: Add Description**|
|publishingType|onPremisesPublishingType|**TODO: Add Description**. Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `intunePfx`, `oflineDomainJoin`, `unknownFutureValue`.|



## Response
If successful, this method returns a `201 Created` response code and a [publishedResource](../resources/publishedresource.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_publishedresource_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}/publishedResources
Content-Type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.publishedResource",
  "displayName": "Display Name value",
  "resourceName": "Resource Name value",
  "publishingType": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.publishedresource"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.publishedResource",
  "id": "5a54aea2-aea2-5a54-a2ae-545aa2ae545a",
  "displayName": "Display Name value",
  "resourceName": "Resource Name value",
  "publishingType": "String"
}
```

