---
title: "Update jobs"
description: "Update the properties of a jobs object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update jobs

Namespace: microsoft.graph

Update the properties of a jobs object.

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
PATCH /applications/{applicationsId}/synchronization/jobs
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [synchronizationJob](../resources/synchronizationjob.md) object.

The following table shows the properties that are required when you create the [synchronizationJob](../resources/synchronizationjob.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|templateId|String|**TODO: Add Description**|
|schedule|[synchronizationSchedule](../resources/synchronizationschedule.md)|**TODO: Add Description**|
|status|[synchronizationStatus](../resources/synchronizationstatus.md)|**TODO: Add Description**|
|synchronizationJobSettings|[keyValuePair](../resources/keyvaluepair.md) collection|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [synchronizationJob](../resources/synchronizationjob.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_jobs"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization/jobs
Content-Type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.synchronizationJob",
  "templateId": "String",
  "schedule": {
    "@odata.type": "microsoft.graph.synchronizationSchedule"
  },
  "status": {
    "@odata.type": "microsoft.graph.synchronizationStatus"
  },
  "synchronizationJobSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ]
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
  "@odata.type": "#microsoft.graph.synchronizationJob",
  "id": "309d63e8-63e8-309d-e863-9d30e8639d30",
  "templateId": "String",
  "schedule": {
    "@odata.type": "microsoft.graph.synchronizationSchedule"
  },
  "status": {
    "@odata.type": "microsoft.graph.synchronizationStatus"
  },
  "synchronizationJobSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ]
}
```

