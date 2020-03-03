---
title: "Update provisioningObjectSummary"
description: "Update the properties of a provisioningObjectSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update provisioningObjectSummary

Namespace: microsoft.graph

Update the properties of a [provisioningObjectSummary](../resources/provisioningobjectsummary.md) object.

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
PATCH /auditLogs/provisioning/{provisioningObjectSummaryId}
PATCH /auditLogs/directoryProvisioning/{provisioningObjectSummaryId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [provisioningObjectSummary](../resources/provisioningobjectsummary.md) object.

The following table shows the properties that are required when you create the [provisioningObjectSummary](../resources/provisioningobjectsummary.md).

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
|sourceSystem|[provisioningSystemDetails](../resources/provisioningsystemdetails.md)||
|targetSystem|[provisioningSystemDetails](../resources/provisioningsystemdetails.md)||
|sourceIdentity|[provisionedIdentity](../resources/provisionedidentity.md)||
|targetIdentity|[provisionedIdentity](../resources/provisionedidentity.md)||
|statusInfo|[statusBase](../resources/statusbase.md)||
|provisioningSteps|[provisioningStep](../resources/provisioningstep.md) collection||
|modifiedProperties|[modifiedProperty](../resources/modifiedproperty.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [provisioningObjectSummary](../resources/provisioningobjectsummary.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_provisioningobjectsummary"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/auditLogs/provisioning/{provisioningObjectSummaryId}
Content-type: application/json
Content-length: 1460

{
  "@odata.type": "#microsoft.graph.provisioningObjectSummary",
  "activityDateTime": "2016-12-31T23:57:38.3073089+03:00",
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1509

{
  "@odata.type": "#microsoft.graph.provisioningObjectSummary",
  "id": "36c378ea-78ea-36c3-ea78-c336ea78c336",
  "activityDateTime": "2016-12-31T23:57:38.3073089+03:00",
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

