---
title: "Add agentGroups"
description: "Add agentGroups by posting to the agentGroups collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add agentGroups

Namespace: microsoft.graph

Add agentGroups by posting to the agentGroups collection.

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
POST /onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}/agents/{onPremisesAgentId}/agentGroups/{onPremisesAgentGroupId}/publishedResources/{publishedResourceId}/agentGroups/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.

The following table shows the properties that are required when you create the [onPremisesAgentGroup](../resources/onpremisesagentgroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|publishingType|onPremisesPublishingType|**TODO: Add Description**. Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `intunePfx`, `oflineDomainJoin`, `unknownFutureValue`.|
|isDefault|Boolean|**TODO: Add Description**|



## Response
If successful, this method returns a `204 No Content` response code and an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}/agents/{onPremisesAgentId}/agentGroups/{onPremisesAgentGroupId}/publishedResources/{publishedResourceId}/agentGroups/$ref
Content-Type: application/json
Content-length: 155

{
  "@odata.type": "#microsoft.graph.onPremisesAgentGroup",
  "displayName": "Display Name value",
  "publishingType": "String",
  "isDefault": true
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onpremisesagentgroup"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.onPremisesAgentGroup",
  "id": "cf1433bd-33bd-cf14-bd33-14cfbd3314cf",
  "displayName": "Display Name value",
  "publishingType": "String",
  "isDefault": true
}
```

