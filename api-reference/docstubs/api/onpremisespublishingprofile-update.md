---
title: "Update onPremisesPublishingProfile"
description: "Update the properties of an onPremisesPublishingProfile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update onPremisesPublishingProfile

Namespace: microsoft.graph

Update the properties of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.

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
PATCH /onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.

The following table shows the properties that are required when you create the [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|hybridAgentUpdaterConfiguration|[hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}
Content-Type: application/json
Content-length: 483

{
  "@odata.type": "#microsoft.graph.onPremisesPublishingProfile",
  "hybridAgentUpdaterConfiguration": {
    "@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration",
    "deferUpdateDateTime": "2017-01-01T00:00:48.4062989+03:00",
    "updateWindow": {
      "@odata.type": "microsoft.graph.updateWindow",
      "updateWindowStartTime": "12:01:47.4800000",
      "updateWindowEndTime": "12:02:47.9810000"
    },
    "allowUpdateConfigurationOverride": true
  }
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
  "@odata.type": "#microsoft.graph.onPremisesPublishingProfile",
  "id": "70ed8b61-8b61-70ed-618b-ed70618bed70",
  "hybridAgentUpdaterConfiguration": {
    "@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration",
    "deferUpdateDateTime": "2017-01-01T00:00:48.4062989+03:00",
    "updateWindow": {
      "@odata.type": "microsoft.graph.updateWindow",
      "updateWindowStartTime": "12:01:47.4800000",
      "updateWindowEndTime": "12:02:47.9810000"
    },
    "allowUpdateConfigurationOverride": true
  }
}
```

