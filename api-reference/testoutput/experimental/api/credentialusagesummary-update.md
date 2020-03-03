---
title: "Update credentialUsageSummary"
description: "Update the properties of a credentialUsageSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update credentialUsageSummary

Update the properties of a [credentialUsageSummary](../resources/credentialusagesummary.md) object.

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
PATCH ** Entity URI for microsoft.graph.credentialUsageSummary not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [credentialUsageSummary](../resources/credentialUsageSummary.md) object.

The following table shows the properties that are required when you create the [credentialUsageSummary](../resources/credentialusagesummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|feature|Enumeration|. Possible values are: `registration`, `reset`, `unknownFutureValue`.|
|successfulActivityCount|Int64||
|failureActivityCount|Int64||
|authMethod|Enumeration|. Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion`, `appNotification`, `appCode`, `alternateMobileCall`, `fido`, `appPassword`, `unknownFutureValue`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [credentialUsageSummary](../resources/credentialusagesummary.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_credentialusagesummary"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.credentialUsageSummary not found
Content-type: application/json
Content-length: 178

{
  "@odata.type": "#microsoft.graph.credentialUsageSummary",
  "feature": "String",
  "successfulActivityCount": 7,
  "failureActivityCount": 4,
  "authMethod": "String"
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
Content-Length: 227

{
  "@odata.type": "#microsoft.graph.credentialUsageSummary",
  "id": "03d92e79-2e79-03d9-792e-d903792ed903",
  "feature": "String",
  "successfulActivityCount": 7,
  "failureActivityCount": 4,
  "authMethod": "String"
}
```

