---
title: "Create provisioningObjectSummary"
description: "Create a new provisioningObjectSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create provisioningObjectSummary

Create a new [provisioningObjectSummary](../resources/provisioningobjectsummary.md) object.

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
POST /auditLogs/provisioning
POST /auditLogs/directoryProvisioning
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the provisioningObjectSummary object.

The following table shows the properties that are required when you create the provisioningObjectSummary.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|activityDateTime|DateTimeOffset||
|tenantId|String||
|jobId|String||
|cycleId|String||
|changeId|String||
|action|String||
|durationInMilliseconds|Int32||
|initiatedBy|[initiator](../resources/initiator.md)||
|sourceSystem|[provisioningSystemDetails](../resources/provisioningSystemDetails.md)||
|targetSystem|[provisioningSystemDetails](../resources/provisioningSystemDetails.md)||
|sourceIdentity|[provisionedIdentity](../resources/provisionedIdentity.md)||
|targetIdentity|[provisionedIdentity](../resources/provisionedIdentity.md)||
|statusInfo|[statusBase](../resources/statusBase.md)||
|provisioningSteps|[provisioningStep](../resources/provisioningStep.md) collection||
|modifiedProperties|[modifiedProperty](../resources/modifiedProperty.md) collection||



## Response
If successful, this method returns a `201 Created` response code and a [provisioningObjectSummary](../resources/provisioningobjectsummary.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_provisioningobjectsummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/auditLogs/provisioning
Content-type: application/json
Content-length: 1460

{
  "@odata.type": "#microsoft.graph.provisioningObjectSummary",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.provisioningobjectsummary"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1509

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
```

