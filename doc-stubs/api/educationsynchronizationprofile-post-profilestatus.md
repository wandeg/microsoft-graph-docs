---
title: "Create profileStatus"
description: "Create a new profileStatus object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create profileStatus

Namespace: microsoft.graph

Create a new profileStatus object.

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
POST /education/synchronizationProfiles/{educationSynchronizationProfileId}/profileStatus
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md) object.

The following table shows the properties that are required when you create the [educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|status|educationSynchronizationStatus|**TODO: Add Description**. Possible values are: `paused`, `inProgress`, `success`, `error`, `validationError`, `quarantined`, `unknownFutureValue`.|
|lastSynchronizationDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_educationsynchronizationprofilestatus_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{educationSynchronizationProfileId}/profileStatus
Content-Type: application/json
Content-length: 158

{
  "@odata.type": "#microsoft.graph.educationSynchronizationProfileStatus",
  "status": "String",
  "lastSynchronizationDateTime": "String (timestamp)"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationsynchronizationprofilestatus"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.educationSynchronizationProfileStatus",
  "id": "73338385-8385-7333-8583-337385833373",
  "status": "String",
  "lastSynchronizationDateTime": "String (timestamp)"
}
```

