---
title: "Get synchronizationJob"
description: "Read the properties and relationships of a synchronizationJob object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get synchronizationJob

Namespace: microsoft.graph

Read the properties and relationships of a [synchronizationJob](../resources/synchronizationjob.md) object.

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
GET /applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [synchronizationJob](../resources/synchronizationjob.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}
-->
``` http
GET https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.synchronizationJob",
    "id": "4960579f-579f-4960-9f57-60499f576049",
    "templateId": "Template Id value",
    "schedule": {
      "@odata.type": "microsoft.graph.synchronizationSchedule",
      "expiration": "2017-01-01T00:00:47.3751057+03:00",
      "interval": "-PT51.0310718S",
      "state": "String"
    },
    "status": {
      "@odata.type": "microsoft.graph.synchronizationStatus",
      "countSuccessiveCompleteFailures": 15,
      "escrowsPruned": true,
      "code": "String",
      "lastExecution": {
        "@odata.type": "microsoft.graph.synchronizationTaskExecution",
        "activityIdentifier": "Activity Identifier value",
        "countEntitled": 13,
        "countEntitledForProvisioning": 12,
        "countEscrowed": 13,
        "countEscrowedRaw": 0,
        "countExported": 13,
        "countExports": 12,
        "countImported": 13,
        "countImportedDeltas": 3,
        "countImportedReferenceDeltas": 12,
        "state": "String",
        "error": {
          "@odata.type": "microsoft.graph.synchronizationError",
          "code": "Code value",
          "message": "Message value",
          "tenantActionable": true
        },
        "timeBegan": "2017-01-01T00:03:25.9506468+03:00",
        "timeEnded": "2017-01-01T00:01:16.0434991+03:00"
      },
      "lastSuccessfulExecution": {
        "@odata.type": "microsoft.graph.synchronizationTaskExecution"
      },
      "lastSuccessfulExecutionWithExports": {
        "@odata.type": "microsoft.graph.synchronizationTaskExecution"
      },
      "progress": [
        {
          "@odata.type": "microsoft.graph.synchronizationProgress",
          "completedUnits": 14,
          "progressObservationDateTime": "2017-01-01T00:00:38.249831+03:00",
          "totalUnits": 10,
          "units": "Units value"
        }
      ],
      "quarantine": {
        "@odata.type": "microsoft.graph.synchronizationQuarantine",
        "currentBegan": "2016-12-31T23:56:32.8554068+03:00",
        "nextAttempt": "2017-01-01T00:03:24.4830453+03:00",
        "reason": "String",
        "seriesBegan": "2017-01-01T00:01:40.2876656+03:00",
        "seriesCount": 11
      },
      "steadyStateFirstAchievedTime": "2017-01-01T00:00:36.123175+03:00",
      "steadyStateLastAchievedTime": "2016-12-31T23:58:46.0546533+03:00",
      "synchronizedEntryCountByType": [
        {
          "@odata.type": "microsoft.graph.stringKeyLongValuePair",
          "key": "Key value",
          "value": 5
        }
      ],
      "troubleshootingUrl": "https://example.com/troubleshootingUrl/"
    },
    "synchronizationJobSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ]
  }
}
```

