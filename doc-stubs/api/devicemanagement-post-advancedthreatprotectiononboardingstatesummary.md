---
title: "Create advancedThreatProtectionOnboardingStateSummary"
description: "Create a new advancedThreatProtectionOnboardingStateSummary object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create advancedThreatProtectionOnboardingStateSummary

Namespace: microsoft.graph

Create a new advancedThreatProtectionOnboardingStateSummary object.

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
POST /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md) object.

The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|unknownDeviceCount|Int32|**TODO: Add Description**|
|notApplicableDeviceCount|Int32|**TODO: Add Description**|
|compliantDeviceCount|Int32|**TODO: Add Description**|
|remediatedDeviceCount|Int32|**TODO: Add Description**|
|nonCompliantDeviceCount|Int32|**TODO: Add Description**|
|errorDeviceCount|Int32|**TODO: Add Description**|
|conflictDeviceCount|Int32|**TODO: Add Description**|
|notAssignedDeviceCount|Int32|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_advancedthreatprotectiononboardingstatesummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary
Content-Type: application/json
Content-length: 395

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "unknownDeviceCount": "Integer",
  "notApplicableDeviceCount": "Integer",
  "compliantDeviceCount": "Integer",
  "remediatedDeviceCount": "Integer",
  "nonCompliantDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "conflictDeviceCount": "Integer",
  "notAssignedDeviceCount": "Integer"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.advancedthreatprotectiononboardingstatesummary"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "id": "918d0262-0262-918d-6202-8d9162028d91",
  "unknownDeviceCount": "Integer",
  "notApplicableDeviceCount": "Integer",
  "compliantDeviceCount": "Integer",
  "remediatedDeviceCount": "Integer",
  "nonCompliantDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "conflictDeviceCount": "Integer",
  "notAssignedDeviceCount": "Integer"
}
```

