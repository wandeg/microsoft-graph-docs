---
title: "Update directoryProvisioning"
description: "Update the properties of a directoryProvisioning object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update directoryProvisioning
Namespace: microsoft.graph

Update the properties of a directoryProvisioning object.

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
PATCH /auditLogs/directoryProvisioning
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [provisioningObjectSummary](../resources/provisioningobjectsummary.md) object.

The following table shows the properties that are required when you create the [provisioningObjectSummary](../resources/provisioningobjectsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|activityDateTime|DateTimeOffset|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|
|jobId|String|**TODO: Add Description**|
|cycleId|String|**TODO: Add Description**|
|changeId|String|**TODO: Add Description**|
|action|String|**TODO: Add Description**|
|durationInMilliseconds|Int32|**TODO: Add Description**|
|servicePrincipal|[provisioningServicePrincipal](../resources/provisioningserviceprincipal.md)|**TODO: Add Description**|
|initiatedBy|[initiator](../resources/initiator.md)|**TODO: Add Description**|
|sourceSystem|[provisioningSystemDetails](../resources/provisioningsystemdetails.md)|**TODO: Add Description**|
|targetSystem|[provisioningSystemDetails](../resources/provisioningsystemdetails.md)|**TODO: Add Description**|
|sourceIdentity|[provisionedIdentity](../resources/provisionedidentity.md)|**TODO: Add Description**|
|targetIdentity|[provisionedIdentity](../resources/provisionedidentity.md)|**TODO: Add Description**|
|statusInfo|[statusBase](../resources/statusbase.md)|**TODO: Add Description**|
|provisioningSteps|[provisioningStep](../resources/provisioningstep.md) collection|**TODO: Add Description**|
|modifiedProperties|[modifiedProperty](../resources/modifiedproperty.md) collection|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [provisioningObjectSummary](../resources/provisioningobjectsummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_directoryprovisioning"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/auditLogs/directoryProvisioning
Content-Type: application/json
Content-length: 1080

{
  "@odata.type": "#microsoft.graph.provisioningObjectSummary",
  "activityDateTime": "String (timestamp)",
  "tenantId": "String",
  "jobId": "String",
  "cycleId": "String",
  "changeId": "String",
  "action": "String",
  "durationInMilliseconds": "Integer",
  "servicePrincipal": {
    "@odata.type": "microsoft.graph.provisioningServicePrincipal"
  },
  "initiatedBy": {
    "@odata.type": "microsoft.graph.initiator"
  },
  "sourceSystem": {
    "@odata.type": "microsoft.graph.provisioningSystemDetails"
  },
  "targetSystem": {
    "@odata.type": "microsoft.graph.provisioningSystemDetails"
  },
  "sourceIdentity": {
    "@odata.type": "microsoft.graph.provisionedIdentity"
  },
  "targetIdentity": {
    "@odata.type": "microsoft.graph.provisionedIdentity"
  },
  "statusInfo": {
    "@odata.type": "microsoft.graph.statusBase"
  },
  "provisioningSteps": [
    {
      "@odata.type": "microsoft.graph.provisioningStep"
    }
  ],
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.modifiedProperty"
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
  "@odata.type": "#microsoft.graph.provisioningObjectSummary",
  "id": "fc3c5262-5262-fc3c-6252-3cfc62523cfc",
  "activityDateTime": "String (timestamp)",
  "tenantId": "String",
  "jobId": "String",
  "cycleId": "String",
  "changeId": "String",
  "action": "String",
  "durationInMilliseconds": "Integer",
  "servicePrincipal": {
    "@odata.type": "microsoft.graph.provisioningServicePrincipal"
  },
  "initiatedBy": {
    "@odata.type": "microsoft.graph.initiator"
  },
  "sourceSystem": {
    "@odata.type": "microsoft.graph.provisioningSystemDetails"
  },
  "targetSystem": {
    "@odata.type": "microsoft.graph.provisioningSystemDetails"
  },
  "sourceIdentity": {
    "@odata.type": "microsoft.graph.provisionedIdentity"
  },
  "targetIdentity": {
    "@odata.type": "microsoft.graph.provisionedIdentity"
  },
  "statusInfo": {
    "@odata.type": "microsoft.graph.statusBase"
  },
  "provisioningSteps": [
    {
      "@odata.type": "microsoft.graph.provisioningStep"
    }
  ],
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.modifiedProperty"
    }
  ]
}
```

