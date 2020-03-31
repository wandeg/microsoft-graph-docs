---
title: "Get onPremisesPublishingProfile"
description: "Read properties and relationships of the onPremisesPublishingProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get onPremisesPublishingProfile

Namespace: microsoft.graph

Read properties and relationships of the [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.

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
GET /onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}
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
If successful, this method returns a `200 OK` response code and [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_onpremisespublishingprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 575

{
  "value": {
    "@odata.type": "#microsoft.graph.onPremisesPublishingProfile",
    "id": "2e61fb21-fb21-2e61-21fb-612e21fb612e",
    "hybridAgentUpdaterConfiguration": {
      "@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration",
      "deferUpdateDateTime": "2017-01-01T00:02:14.3622262+03:00",
      "updateWindow": {
        "@odata.type": "microsoft.graph.updateWindow",
        "updateWindowStartTime": "11:59:13.7280000",
        "updateWindowEndTime": "12:02:16.7390000"
      },
      "allowUpdateConfigurationOverride": true
    }
  }
}
```

