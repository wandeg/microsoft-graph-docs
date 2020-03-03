---
title: "List onPremisesPublishingProfiles"
description: "List properties and relationships of the onPremisesPublishingProfile objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List onPremisesPublishingProfiles

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
GET https://graph.microsoft.com/docs\api/onPremisesPublishingProfiles
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
Content-Length: 613

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.onPremisesPublishingProfile",
      "id": "ad1876c2-76c2-ad18-c276-18adc27618ad",
      "hybridAgentUpdaterConfiguration": {
        "@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration",
        "deferUpdateDateTime": "2017-01-01T00:02:44.2681456+03:00",
        "updateWindow": {
          "@odata.type": "microsoft.graph.updateWindow",
          "updateWindowStartTime": "11:56:41.9540000",
          "updateWindowEndTime": "11:56:40.5520000"
        },
        "allowUpdateConfigurationOverride": true
      }
    }
  ]
}
```

