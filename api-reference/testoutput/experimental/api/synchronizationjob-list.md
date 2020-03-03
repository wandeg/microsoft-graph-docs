---
title: "List synchronizationJobs"
description: "List properties and relationships of the synchronizationJob objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List synchronizationJobs

Namespace: microsoft.graph

List properties and relationships of the [synchronizationJob](../resources/synchronizationjob.md) objects.

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
GET /applications/{applicationsId}/synchronization/jobs
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronizationjob.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}
-->
``` http
GET https://graph.microsoft.com/localtest/applications/{applicationsId}/synchronization/jobs
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.synchronizationjob)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3046

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.synchronizationJob",
      "id": "b8997069-7069-b899-6970-99b8697099b8",
      "templateId": "Template Id value",
      "schedule": {
        "@odata.type": "microsoft.graph.synchronizationSchedule",
        "expiration": "2016-12-31T23:57:48.0321632+03:00",
        "interval": "-PT2M35.6823926S",
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
          "timeBegan": "2016-12-31T23:56:38.758188+03:00",
          "timeEnded": "2017-01-01T00:00:59.4792075+03:00"
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
            "progressObservationDateTime": "2016-12-31T23:58:06.548007+03:00",
            "totalUnits": 10,
            "units": "Units value"
          }
        ],
        "quarantine": {
          "@odata.type": "microsoft.graph.synchronizationQuarantine",
          "currentBegan": "2016-12-31T23:57:24.2893083+03:00",
          "nextAttempt": "2016-12-31T23:59:51.872306+03:00",
          "reason": "String",
          "seriesBegan": "2017-01-01T00:00:37.242502+03:00",
          "seriesCount": 11
        },
        "steadyStateFirstAchievedTime": "2016-12-31T23:57:16.2528743+03:00",
        "steadyStateLastAchievedTime": "2016-12-31T23:59:10.0513884+03:00",
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
  ]
}
```

