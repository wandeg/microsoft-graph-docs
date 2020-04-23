---
title: "Update deviceCompliancePolicies"
description: "Update the properties of a deviceCompliancePolicies object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update deviceCompliancePolicies

Namespace: microsoft.graph

Update the properties of a deviceCompliancePolicies object.

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
PATCH /deviceManagement/deviceCompliancePolicies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [deviceCompliancePolicy](../resources/devicecompliancepolicy.md) object.

The following table shows the properties that are required when you create the [deviceCompliancePolicy](../resources/devicecompliancepolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created.|
|description|String|Admin provided description of the Device Configuration.|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|displayName|String|Admin provided name of the device configuration.|
|version|Int32|Version of the device configuration.|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicy](../resources/devicecompliancepolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_devicecompliancepolicies"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-Type: application/json
Content-length: 160

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
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
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "id": "14cbca29-ca29-14cb-29ca-cb1429cacb14",
  "createdDateTime": "2017-01-01T00:02:24.9669049+03:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:02:46.687785+03:00",
  "displayName": "Display Name value",
  "version": 7
}
```

