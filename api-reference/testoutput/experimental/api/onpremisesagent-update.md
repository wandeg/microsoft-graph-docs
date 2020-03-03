---
title: "Update onPremisesAgent"
description: "Update the properties of a onPremisesAgent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update onPremisesAgent

Namespace: microsoft.graph

Update the properties of a [onPremisesAgent](../resources/onpremisesagent.md) object.

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
PATCH /onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}/agents/{onPremisesAgentId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [onPremisesAgent](../resources/onpremisesagent.md) object.

The following table shows the properties that are required when you create the [onPremisesAgent](../resources/onpremisesagent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|machineName|String||
|externalIp|String||
|status|Enumeration|. Possible values are: `active`, `inactive`.|
|supportedPublishingTypes|Enumeration collection|. Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `intunePfx`, `oflineDomainJoin`, `unknownFutureValue`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [onPremisesAgent](../resources/onpremisesagent.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_onpremisesagent"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}/agents/{onPremisesAgentId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.onPremisesAgent",
  "id": "97e9ae49-ae49-97e9-49ae-e99749aee997",
  "machineName": "Machine Name value",
  "externalIp": "External Ip value",
  "status": "String",
  "supportedPublishingTypes": [
    "String"
  ]
}
```

