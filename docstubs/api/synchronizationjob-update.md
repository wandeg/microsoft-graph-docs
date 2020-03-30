---
title: "Update synchronizationJob"
description: "Update the properties of a synchronizationJob object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update synchronizationJob

Namespace: microsoft.graph

Update the properties of a [synchronizationJob](../resources/synchronizationjob.md) object.

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
PATCH /applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [synchronizationJob](../resources/synchronizationjob.md) object.

The following table shows the properties that are required when you create the [synchronizationJob](../resources/synchronizationjob.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|templateId|String||
|schedule|[synchronizationSchedule](../resources/synchronizationschedule.md)||
|status|[synchronizationStatus](../resources/synchronizationstatus.md)||
|synchronizationJobSettings|[keyValuePair](../resources/keyvaluepair.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [synchronizationJob](../resources/synchronizationjob.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_synchronizationjob"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}
Content-type: application/json
Content-length: 2659

{
  "@odata.type": "#microsoft.graph.synchronizationJob",
  "templateId": "Template Id value",
  "schedule": {
    "@odata.type": "microsoft.graph.synchronizationSchedule",
    "expiration": "2017-01-01T00:01:08.1940627+03:00",
    "interval": "-PT2M5.3636489S",
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
      "timeBegan": "2017-01-01T00:02:17.0925057+03:00",
      "timeEnded": "2016-12-31T23:57:29.9700132+03:00"
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
        "progressObservationDateTime": "2016-12-31T23:59:28.4022048+03:00",
        "totalUnits": 10,
        "units": "Units value"
      }
    ],
    "quarantine": {
      "@odata.type": "microsoft.graph.synchronizationQuarantine",
      "currentBegan": "2016-12-31T23:58:01.3982502+03:00",
      "nextAttempt": "2017-01-01T00:00:00.0575165+03:00",
      "reason": "String",
      "seriesBegan": "2016-12-31T23:59:43.3562509+03:00",
      "seriesCount": 11
    },
    "steadyStateFirstAchievedTime": "2016-12-31T23:59:23.3145158+03:00",
    "steadyStateLastAchievedTime": "2016-12-31T23:57:20.4060637+03:00",
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
Content-Length: 2708

{
  "@odata.type": "#microsoft.graph.synchronizationJob",
  "id": "f2430f17-0f17-f243-170f-43f2170f43f2",
  "templateId": "Template Id value",
  "schedule": {
    "@odata.type": "microsoft.graph.synchronizationSchedule",
    "expiration": "2017-01-01T00:01:08.1940627+03:00",
    "interval": "-PT2M5.3636489S",
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
      "timeBegan": "2017-01-01T00:02:17.0925057+03:00",
      "timeEnded": "2016-12-31T23:57:29.9700132+03:00"
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
        "progressObservationDateTime": "2016-12-31T23:59:28.4022048+03:00",
        "totalUnits": 10,
        "units": "Units value"
      }
    ],
    "quarantine": {
      "@odata.type": "microsoft.graph.synchronizationQuarantine",
      "currentBegan": "2016-12-31T23:58:01.3982502+03:00",
      "nextAttempt": "2017-01-01T00:00:00.0575165+03:00",
      "reason": "String",
      "seriesBegan": "2016-12-31T23:59:43.3562509+03:00",
      "seriesCount": 11
    },
    "steadyStateFirstAchievedTime": "2016-12-31T23:59:23.3145158+03:00",
    "steadyStateLastAchievedTime": "2016-12-31T23:57:20.4060637+03:00",
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
```

