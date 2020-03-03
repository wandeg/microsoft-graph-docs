---
title: "Create securityBaselineCategoryStateSummary"
description: "Create a new securityBaselineCategoryStateSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create securityBaselineCategoryStateSummary

Namespace: microsoft.graph

Create a new [securityBaselineCategoryStateSummary](../resources/securitybaselinecategorystatesummary.md) object.

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
POST /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [securityBaselineCategoryStateSummary](../resources/securitybaselinecategorystatesummary.md) object.

The following table shows the properties that are required when you create the [securityBaselineCategoryStateSummary](../resources/securitybaselinecategorystatesummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|secureCount|Int32|Number of secure devices Inherited from [securityBaselineStateSummary](../resources/securitybaselinestatesummary.md)|
|notSecureCount|Int32|Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/securitybaselinestatesummary.md)|
|unknownCount|Int32|Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/securitybaselinestatesummary.md)|
|errorCount|Int32|Number of error devices Inherited from [securityBaselineStateSummary](../resources/securitybaselinestatesummary.md)|
|conflictCount|Int32|Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/securitybaselinestatesummary.md)|
|notApplicableCount|Int32|Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/securitybaselinestatesummary.md)|
|displayName|String|The category name|



## Response
If successful, this method returns a `201 Created` response code and a [securityBaselineCategoryStateSummary](../resources/securitybaselinecategorystatesummary.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_securitybaselinecategorystatesummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
Content-type: application/json
Content-length: 261

{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2,
  "displayName": "Display Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securitybaselinecategorystatesummary"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 310

{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "id": "4a601bdb-1bdb-4a60-db1b-604adb1b604a",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2,
  "displayName": "Display Name value"
}
```

