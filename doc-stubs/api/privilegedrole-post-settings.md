---
title: "Create settings"
description: "Create a new settings object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create settings
Namespace: microsoft.graph

Create a new settings object.

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
POST ** Collection URI for microsoft.graph.privilegedRoleSettings not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.

The following table shows the properties that are required when you create the [privilegedRoleSettings](../resources/privilegedrolesettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|approverIds|String collection|**TODO: Add Description**|
|minElevationDuration|Duration|**TODO: Add Description**|
|maxElavationDuration|Duration|**TODO: Add Description**|
|elevationDuration|Duration|**TODO: Add Description**|
|notificationToUserOnElevation|Boolean|**TODO: Add Description**|
|ticketingInfoOnElevation|Boolean|**TODO: Add Description**|
|mfaOnElevation|Boolean|**TODO: Add Description**|
|lastGlobalAdmin|Boolean|**TODO: Add Description**|
|isMfaOnElevationConfigurable|Boolean|**TODO: Add Description**|
|approvalOnElevation|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_privilegedrolesettings_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.privilegedRoleSettings not found
Content-Type: application/json
Content-length: 482

{
  "@odata.type": "#microsoft.graph.privilegedRoleSettings",
  "approverIds": [
    "String"
  ],
  "minElevationDuration": "String (duration)",
  "maxElavationDuration": "String (duration)",
  "elevationDuration": "String (duration)",
  "notificationToUserOnElevation": "Boolean",
  "ticketingInfoOnElevation": "Boolean",
  "mfaOnElevation": "Boolean",
  "lastGlobalAdmin": "Boolean",
  "isMfaOnElevationConfigurable": "Boolean",
  "approvalOnElevation": "Boolean"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedrolesettings"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.privilegedRoleSettings",
  "id": "b20f5660-5660-b20f-6056-0fb260560fb2",
  "approverIds": [
    "String"
  ],
  "minElevationDuration": "String (duration)",
  "maxElavationDuration": "String (duration)",
  "elevationDuration": "String (duration)",
  "notificationToUserOnElevation": "Boolean",
  "ticketingInfoOnElevation": "Boolean",
  "mfaOnElevation": "Boolean",
  "lastGlobalAdmin": "Boolean",
  "isMfaOnElevationConfigurable": "Boolean",
  "approvalOnElevation": "Boolean"
}
```

