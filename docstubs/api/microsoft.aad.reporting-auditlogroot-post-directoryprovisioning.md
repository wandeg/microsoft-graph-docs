---
title: "Add directoryProvisioning"
description: "Add directoryProvisioning by posting to the directoryProvisioning collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add directoryProvisioning

Namespace: Microsoft.AAD.Reporting

Add directoryProvisioning by posting to the directoryProvisioning collection.

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
POST /auditLogs/directoryProvisioning/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md) object.

The following table shows the properties that are required when you create the [provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String||
|activityDateTime|DateTimeOffset||
|tenantId|String||
|jobId|String||
|cycleId|String||
|changeId|String||
|action|String||
|durationInMilliseconds|Int32||
|initiatedBy|[initiator](../resources/microsoft.aad.reporting-initiator.md)||
|sourceSystem|[provisioningSystemDetails](../resources/microsoft.aad.reporting-provisioningsystemdetails.md)||
|targetSystem|[provisioningSystemDetails](../resources/microsoft.aad.reporting-provisioningsystemdetails.md)||
|sourceIdentity|[provisionedIdentity](../resources/microsoft.aad.reporting-provisionedidentity.md)||
|targetIdentity|[provisionedIdentity](../resources/microsoft.aad.reporting-provisionedidentity.md)||
|statusInfo|[statusBase](../resources/microsoft.aad.reporting-statusbase.md)||
|provisioningSteps|[provisioningStep](../resources/microsoft.aad.reporting-provisioningstep.md) collection||
|modifiedProperties|[modifiedProperty](../resources/microsoft.aad.reporting-modifiedproperty.md) collection||



## Response
If successful, this method returns a `201 Created` response code and a [provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_provisioningobjectsummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/auditLogs/directoryProvisioning
Content-type: application/json
Content-length: 1540

{
  "@odata.type": "#Microsoft.AAD.Reporting.provisioningObjectSummary",
  "activityDateTime": "2016-12-31T23:56:54.8488209+00:00",
  "tenantId": "Tenant Id value",
  "jobId": "Job Id value",
  "cycleId": "Cycle Id value",
  "changeId": "Change Id value",
  "action": "Action value",
  "durationInMilliseconds": 6,
  "initiatedBy": {
    "@odata.type": "Microsoft.AAD.Reporting.initiator",
    "id": "Id value",
    "displayName": "Display Name value",
    "initiatorType": "String"
  },
  "sourceSystem": {
    "@odata.type": "Microsoft.AAD.Reporting.provisioningSystemDetails",
    "details": {
      "@odata.type": "Microsoft.AAD.Reporting.detailsInfo"
    }
  },
  "targetSystem": {
    "@odata.type": "Microsoft.AAD.Reporting.provisioningSystemDetails"
  },
  "sourceIdentity": {
    "@odata.type": "Microsoft.AAD.Reporting.provisionedIdentity",
    "identityType": "Identity Type value"
  },
  "targetIdentity": {
    "@odata.type": "Microsoft.AAD.Reporting.provisionedIdentity"
  },
  "statusInfo": {
    "@odata.type": "Microsoft.AAD.Reporting.statusBase",
    "status": "String"
  },
  "provisioningSteps": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.provisioningStep",
      "name": "Name value",
      "description": "Description value",
      "provisioningStepType": "String"
    }
  ],
  "modifiedProperties": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.modifiedProperty",
      "oldValue": "Old Value value",
      "newValue": "New Value value"
    }
  ]
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.aad.reporting.provisioningobjectsummary"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1589

{
  "@odata.type": "#Microsoft.AAD.Reporting.provisioningObjectSummary",
  "id": "848fa6c0-a6c0-848f-c0a6-8f84c0a68f84",
  "activityDateTime": "2016-12-31T23:56:54.8488209+00:00",
  "tenantId": "Tenant Id value",
  "jobId": "Job Id value",
  "cycleId": "Cycle Id value",
  "changeId": "Change Id value",
  "action": "Action value",
  "durationInMilliseconds": 6,
  "initiatedBy": {
    "@odata.type": "Microsoft.AAD.Reporting.initiator",
    "id": "Id value",
    "displayName": "Display Name value",
    "initiatorType": "String"
  },
  "sourceSystem": {
    "@odata.type": "Microsoft.AAD.Reporting.provisioningSystemDetails",
    "details": {
      "@odata.type": "Microsoft.AAD.Reporting.detailsInfo"
    }
  },
  "targetSystem": {
    "@odata.type": "Microsoft.AAD.Reporting.provisioningSystemDetails"
  },
  "sourceIdentity": {
    "@odata.type": "Microsoft.AAD.Reporting.provisionedIdentity",
    "identityType": "Identity Type value"
  },
  "targetIdentity": {
    "@odata.type": "Microsoft.AAD.Reporting.provisionedIdentity"
  },
  "statusInfo": {
    "@odata.type": "Microsoft.AAD.Reporting.statusBase",
    "status": "String"
  },
  "provisioningSteps": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.provisioningStep",
      "name": "Name value",
      "description": "Description value",
      "provisioningStepType": "String"
    }
  ],
  "modifiedProperties": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.modifiedProperty",
      "oldValue": "Old Value value",
      "newValue": "New Value value"
    }
  ]
}
```

