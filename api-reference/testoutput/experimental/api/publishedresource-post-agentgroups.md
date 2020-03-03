---
title: "Create agentGroups"
description: "Create agentGroups by posting to the agentGroups collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create agentGroups

Create agentGroups by posting to the agentGroups collection.

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
POST /onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}/agents/{onPremisesAgentId}/agentGroups/{onPremisesAgentGroupId}/publishedResources/{publishedResourceId}/agentGroups/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the onPremisesAgentGroup object.

The following table shows the properties that are required when you create the onPremisesAgentGroup.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|publishingType|Enumeration|. Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `intunePfx`, `oflineDomainJoin`, `unknownFutureValue`.|
|isDefault|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}/agents/{onPremisesAgentId}/agentGroups/{onPremisesAgentGroupId}/publishedResources/{publishedResourceId}/agentGroups
Content-type: application/json
Content-length: 155

{
  "@odata.type": "#microsoft.graph.onPremisesAgentGroup",
  "displayName": "Display Name value",
  "publishingType": "String",
  "isDefault": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onpremisesagentgroup"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 204

{
  "@odata.type": "#microsoft.graph.onPremisesAgentGroup",
  "id": "7b1dc0c4-c0c4-7b1d-c4c0-1d7bc4c01d7b",
  "displayName": "Display Name value",
  "publishingType": "String",
  "isDefault": true
}
```

