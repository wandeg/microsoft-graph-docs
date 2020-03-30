---
title: "Create onPremisesPublishingProfile"
description: "Create a new onPremisesPublishingProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create onPremisesPublishingProfile

Namespace: microsoft.graph

Create a new [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.

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
POST /onPremisesPublishingProfiles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.

The following table shows the properties that are required when you create the [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|hybridAgentUpdaterConfiguration|[hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md)||



## Response
If successful, this method returns a `201 Created` response code and a [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_onpremisespublishingprofile_from_onpremisespublishingprofiles"
}
-->
``` http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles
Content-type: application/json
Content-length: 483

{
  "@odata.type": "#microsoft.graph.onPremisesPublishingProfile",
  "hybridAgentUpdaterConfiguration": {
    "@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration",
    "deferUpdateDateTime": "2017-01-01T00:00:29.4625982+03:00",
    "updateWindow": {
      "@odata.type": "microsoft.graph.updateWindow",
      "updateWindowStartTime": "12:01:47.4060000",
      "updateWindowEndTime": "11:56:57.0270000"
    },
    "allowUpdateConfigurationOverride": true
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onpremisespublishingprofile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 532

{
  "@odata.type": "#microsoft.graph.onPremisesPublishingProfile",
  "id": "db7cabfa-abfa-db7c-faab-7cdbfaab7cdb",
  "hybridAgentUpdaterConfiguration": {
    "@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration",
    "deferUpdateDateTime": "2017-01-01T00:00:29.4625982+03:00",
    "updateWindow": {
      "@odata.type": "microsoft.graph.updateWindow",
      "updateWindowStartTime": "12:01:47.4060000",
      "updateWindowEndTime": "11:56:57.0270000"
    },
    "allowUpdateConfigurationOverride": true
  }
}
```

