---
title: "Create credentialUsageSummary"
description: "Create a new credentialUsageSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create credentialUsageSummary

Namespace: microsoft.graph

Create a new [credentialUsageSummary](../resources/credentialusagesummary.md) object.

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
POST ** Collection URI for microsoft.graph.credentialUsageSummary not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [credentialUsageSummary](../resources/credentialusagesummary.md) object.

The following table shows the properties that are required when you create the [credentialUsageSummary](../resources/credentialusagesummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|feature|Enumeration|. Possible values are: `registration`, `reset`, `unknownFutureValue`.|
|successfulActivityCount|Int64||
|failureActivityCount|Int64||
|authMethod|Enumeration|. Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion`, `appNotification`, `appCode`, `alternateMobileCall`, `fido`, `appPassword`, `unknownFutureValue`.|



## Response
If successful, this method returns a `201 Created` response code and a [credentialUsageSummary](../resources/credentialusagesummary.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_credentialusagesummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.credentialUsageSummary not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialusagesummary"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 227

{
  "@odata.type": "#microsoft.graph.credentialUsageSummary",
  "id": "83519856-9856-8351-5698-518356985183",
  "feature": "String",
  "successfulActivityCount": 7,
  "failureActivityCount": 4,
  "authMethod": "String"
}
```

