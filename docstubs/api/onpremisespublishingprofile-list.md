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

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /onPremisesPublishingProfiles
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
If successful, this method returns a `200 OK` response code and a collection of [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_onpremisespublishingprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles
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
      "id": "b8b586d5-86d5-b8b5-d586-b5b8d586b5b8",
      "hybridAgentUpdaterConfiguration": {
        "@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration",
        "deferUpdateDateTime": "2017-01-01T00:01:56.7448349+00:00",
        "updateWindow": {
          "@odata.type": "microsoft.graph.updateWindow",
          "updateWindowStartTime": "12:00:43.5930000",
          "updateWindowEndTime": "11:57:53.0500000"
        },
        "allowUpdateConfigurationOverride": true
      }
    }
  ]
}
```

