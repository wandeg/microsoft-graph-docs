---
title: "Add deviceCompliancePolicies"
description: "Add deviceCompliancePolicies by posting to the deviceCompliancePolicies collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add deviceCompliancePolicies

Namespace: microsoft.graph

Add deviceCompliancePolicies by posting to the deviceCompliancePolicies collection.

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
POST /deviceManagement/deviceCompliancePolicies/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceCompliancePolicy](../resources/devicecompliancepolicy.md) object.

The following table shows the properties that are required when you create the [deviceCompliancePolicy](../resources/devicecompliancepolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|roleScopeTagIds|String collection||
|createdDateTime|DateTimeOffset||
|description|String||
|lastModifiedDateTime|DateTimeOffset||
|displayName|String||
|version|Int32||



## Response
If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicy](../resources/devicecompliancepolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicecompliancepolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 222

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicecompliancepolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 393

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "id": "faa3ad86-ad86-faa3-86ad-a3fa86ada3fa",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "createdDateTime": "2016-12-31T23:58:10.4520456+03:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:02:23.471109+03:00",
  "displayName": "Display Name value",
  "version": 7
}
```

