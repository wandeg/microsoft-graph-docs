---
title: "List provisioning"
description: "Get the provisioningObjectSummaries from the provisioning navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List provisioning

Get the provisioningObjectSummaries from the provisioning navigation property.

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
GET /auditLogs/provisioning
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [provisioningObjectSummary](../resources/provisioningobjectsummary.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_provisioningobjectsummary"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/auditLogs/provisioning
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.provisioningobjectsummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1742

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.provisioningObjectSummary",
      "id": "f4228028-8028-f422-2880-22f4288022f4",
      "activityDateTime": "2017-01-01T00:02:10.8639373+03:00",
      "tenantId": "Tenant Id value",
      "jobId": "Job Id value",
      "cycleId": "Cycle Id value",
      "changeId": "Change Id value",
      "action": "Action value",
      "durationInMilliseconds": 6,
      "initiatedBy": {
        "@odata.type": "microsoft.graph.initiator",
        "id": "Id value",
        "displayName": "Display Name value",
        "initiatorType": "String"
      },
      "sourceSystem": {
        "@odata.type": "microsoft.graph.provisioningSystemDetails",
        "details": {
          "@odata.type": "microsoft.graph.detailsInfo"
        }
      },
      "targetSystem": {
        "@odata.type": "microsoft.graph.provisioningSystemDetails"
      },
      "sourceIdentity": {
        "@odata.type": "microsoft.graph.provisionedIdentity",
        "identityType": "Identity Type value"
      },
      "targetIdentity": {
        "@odata.type": "microsoft.graph.provisionedIdentity"
      },
      "statusInfo": {
        "@odata.type": "microsoft.graph.statusBase",
        "status": "String"
      },
      "provisioningSteps": [
        {
          "@odata.type": "microsoft.graph.provisioningStep",
          "name": "Name value",
          "description": "Description value",
          "provisioningStepType": "String"
        }
      ],
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.modifiedProperty",
          "oldValue": "Old Value value",
          "newValue": "New Value value"
        }
      ]
    }
  ]
}
```

