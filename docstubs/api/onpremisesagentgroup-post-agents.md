---
title: "Create agents"
description: "Create agents by posting to the agents collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create agents

Namespace: microsoft.graph

Create agents by posting to the agents collection.

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
POST /onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}/agents/{onPremisesAgentId}/agentGroups/{onPremisesAgentGroupId}/agents/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [onPremisesAgent](../resources/onpremisesagent.md) object.

The following table shows the properties that are required when you create the [onPremisesAgent](../resources/onpremisesagent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|machineName|String||
|externalIp|String||
|status|Enumeration| Possible values are: `active`, `inactive`.|
|supportedPublishingTypes|Enumeration collection| Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `intunePfx`, `oflineDomainJoin`, `unknownFutureValue`.|



## Response
If successful, this method returns a `201 Created` response code and a [onPremisesAgent](../resources/onpremisesagent.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagent_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}/agents/{onPremisesAgentId}/agentGroups/{onPremisesAgentGroupId}/agents
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.onPremisesAgent",
  "machineName": "Machine Name value",
  "externalIp": "External Ip value",
  "status": "String",
  "supportedPublishingTypes": [
    "String"
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onpremisesagent"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.onPremisesAgent",
  "id": "816accaf-ccaf-816a-afcc-6a81afcc6a81",
  "machineName": "Machine Name value",
  "externalIp": "External Ip value",
  "status": "String",
  "supportedPublishingTypes": [
    "String"
  ]
}
```

