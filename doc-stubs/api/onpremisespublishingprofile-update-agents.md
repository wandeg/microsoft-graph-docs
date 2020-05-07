---
title: "Update agents"
description: "Update the properties of an agents object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update agents

Namespace: microsoft.graph

Update the properties of an agents object.

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
PATCH /onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}/agents
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [onPremisesAgent](../resources/onpremisesagent.md) object.

The following table shows the properties that are required when you create the [onPremisesAgent](../resources/onpremisesagent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|machineName|String|**TODO: Add Description**|
|externalIp|String|**TODO: Add Description**|
|status|agentStatus|**TODO: Add Description**. Possible values are: `active`, `inactive`.|
|supportedPublishingTypes|onPremisesPublishingType collection|**TODO: Add Description**. Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `intunePfx`, `oflineDomainJoin`, `unknownFutureValue`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [onPremisesAgent](../resources/onpremisesagent.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_agents"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}/agents
Content-Type: application/json
Content-length: 188

{
  "@odata.type": "#microsoft.graph.onPremisesAgent",
  "machineName": "String",
  "externalIp": "String",
  "status": "String",
  "supportedPublishingTypes": [
    "String"
  ]
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
  "@odata.type": "#microsoft.graph.onPremisesAgent",
  "id": "1c40d48e-d48e-1c40-8ed4-401c8ed4401c",
  "machineName": "String",
  "externalIp": "String",
  "status": "String",
  "supportedPublishingTypes": [
    "String"
  ]
}
```

