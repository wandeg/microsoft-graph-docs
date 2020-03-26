---
title: "Update onPremisesPublishingProfile"
description: "Update the properties of a onPremisesPublishingProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update onPremisesPublishingProfile

Namespace: microsoft.graph

Update the properties of a [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.

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
PATCH /onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.

The following table shows the properties that are required when you create the [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|hybridAgentUpdaterConfiguration|[hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}
Content-type: application/json
Content-length: 483

{
  "@odata.type": "#microsoft.graph.onPremisesPublishingProfile",
  "hybridAgentUpdaterConfiguration": {
    "@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration",
    "deferUpdateDateTime": "2017-01-01T00:03:09.5743704+00:00",
    "updateWindow": {
      "@odata.type": "microsoft.graph.updateWindow",
      "updateWindowStartTime": "11:57:13.0640000",
      "updateWindowEndTime": "12:03:07.5420000"
    },
    "allowUpdateConfigurationOverride": true
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 532

{
  "@odata.type": "#microsoft.graph.onPremisesPublishingProfile",
  "id": "d208cb69-cb69-d208-69cb-08d269cb08d2",
  "hybridAgentUpdaterConfiguration": {
    "@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration",
    "deferUpdateDateTime": "2017-01-01T00:03:09.5743704+00:00",
    "updateWindow": {
      "@odata.type": "microsoft.graph.updateWindow",
      "updateWindowStartTime": "11:57:13.0640000",
      "updateWindowEndTime": "12:03:07.5420000"
    },
    "allowUpdateConfigurationOverride": true
  }
}
```

