---
title: "Update profileStatus"
description: "Update the properties of a profileStatus object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update profileStatus

Namespace: microsoft.graph

Update the properties of a profileStatus object.

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
PATCH /education/synchronizationProfiles/{educationSynchronizationProfileId}/profileStatus
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md) object.

The following table shows the properties that are required when you create the [educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|status|educationSynchronizationStatus|**TODO: Add Description**. Possible values are: `paused`, `inProgress`, `success`, `error`, `validationError`, `quarantined`, `unknownFutureValue`.|
|lastSynchronizationDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_profilestatus"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/education/synchronizationProfiles/{educationSynchronizationProfileId}/profileStatus
Content-Type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.educationSynchronizationProfileStatus",
  "status": "String",
  "lastSynchronizationDateTime": "2017-01-01T00:01:37.6538798+03:00"
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
  "@odata.type": "#microsoft.graph.educationSynchronizationProfileStatus",
  "id": "f1e9307b-307b-f1e9-7b30-e9f17b30e9f1",
  "status": "String",
  "lastSynchronizationDateTime": "2017-01-01T00:01:37.6538798+03:00"
}
```

