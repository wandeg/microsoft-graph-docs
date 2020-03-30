---
title: "List agents"
description: "Get the onPremisesAgents from the agents navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List agents

Namespace: microsoft.graph

Get the onPremisesAgents from the agents navigation property.

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
GET /onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}/agents/{onPremisesAgentId}/agentGroups/{onPremisesAgentGroupId}/agents
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [onPremisesAgent](../resources/onpremisesagent.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_onpremisesagent"
}
-->
``` http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}/agents/{onPremisesAgentId}/agentGroups/{onPremisesAgentGroupId}/agents
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.onpremisesagent)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 325

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.onPremisesAgent",
      "id": "d90ef987-f987-d90e-87f9-0ed987f90ed9",
      "machineName": "Machine Name value",
      "externalIp": "External Ip value",
      "status": "String",
      "supportedPublishingTypes": [
        "String"
      ]
    }
  ]
}
```

