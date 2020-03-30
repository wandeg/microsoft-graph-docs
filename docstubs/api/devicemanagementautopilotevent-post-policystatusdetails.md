---
title: "Add policyStatusDetails"
description: "Add policyStatusDetails by posting to the policyStatusDetails collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add policyStatusDetails

Namespace: microsoft.graph

Add policyStatusDetails by posting to the policyStatusDetails collection.

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
POST /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md) object.

The following table shows the properties that are required when you create the [deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|policyType|Enumeration| Possible values are: `unknown`, `application`, `appModel`, `configurationPolicy`.|
|complianceStatus|Enumeration| Possible values are: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.|
|trackedOnEnrollmentStatus|Boolean||
|lastReportedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementautopilotpolicystatusdetail_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails
Content-type: application/json
Content-length: 287

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "displayName": "Display Name value",
  "policyType": "String",
  "complianceStatus": "String",
  "trackedOnEnrollmentStatus": true,
  "lastReportedDateTime": "2016-12-31T23:59:04.0371883+03:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementautopilotpolicystatusdetail"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 336

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "id": "029635fb-35fb-0296-fb35-9602fb359602",
  "displayName": "Display Name value",
  "policyType": "String",
  "complianceStatus": "String",
  "trackedOnEnrollmentStatus": true,
  "lastReportedDateTime": "2016-12-31T23:59:04.0371883+03:00"
}
```

