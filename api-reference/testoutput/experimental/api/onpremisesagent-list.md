---
title: "List onPremisesAgents"
description: "List properties and relationships of the onPremisesAgent objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List onPremisesAgents

List properties and relationships of the [onPremisesAgent](../resources/onpremisesagent.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}/agents
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [onPremisesAgent](../resources/onpremisesagent.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_onpremisesagent"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}/agents
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
      "id": "60031e2b-1e2b-6003-2b1e-03602b1e0360",
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

