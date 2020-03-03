---
title: "Update securityBaselineStateSummary"
description: "Update the properties of a securityBaselineStateSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update securityBaselineStateSummary

Namespace: microsoft.graph

Update the properties of a [securityBaselineStateSummary](../resources/securitybaselinestatesummary.md) object.

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
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [securityBaselineStateSummary](../resources/securitybaselinestatesummary.md) object.

The following table shows the properties that are required when you create the [securityBaselineStateSummary](../resources/securitybaselinestatesummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|secureCount|Int32|Number of secure devices|
|notSecureCount|Int32|Number of not secure devices|
|unknownCount|Int32|Number of unknown devices|
|errorCount|Int32|Number of error devices|
|conflictCount|Int32|Number of conflict devices|
|notApplicableCount|Int32|Number of not applicable devices|



## Response
If successful, this method returns a `200 OK` response code and an updated [securityBaselineStateSummary](../resources/securitybaselinestatesummary.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_securitybaselinestatesummary"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
Content-type: application/json
Content-length: 213

{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2
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
Content-Length: 262

{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "id": "fef4217c-217c-fef4-7c21-f4fe7c21f4fe",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2
}
```

