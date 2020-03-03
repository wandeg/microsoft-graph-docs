---
title: "List onPremisesPublishingProfiles"
description: "List properties and relationships of the onPremisesPublishingProfile objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List onPremisesPublishingProfiles

Namespace: microsoft.graph

List properties and relationships of the [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) objects.

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
GET /onPremisesPublishingProfiles
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_onpremisespublishingprofile"
}
-->
``` http
GET https://graph.microsoft.com/localtest/onPremisesPublishingProfiles
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.onpremisespublishingprofile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 612

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.onPremisesPublishingProfile",
      "id": "6e2a39a7-39a7-6e2a-a739-2a6ea7392a6e",
      "hybridAgentUpdaterConfiguration": {
        "@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration",
        "deferUpdateDateTime": "2017-01-01T00:01:51.697502+03:00",
        "updateWindow": {
          "@odata.type": "microsoft.graph.updateWindow",
          "updateWindowStartTime": "11:56:40.8130000",
          "updateWindowEndTime": "11:59:11.8990000"
        },
        "allowUpdateConfigurationOverride": true
      }
    }
  ]
}
```

