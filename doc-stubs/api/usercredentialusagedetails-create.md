---
title: "Create userCredentialUsageDetails"
description: "Create a new userCredentialUsageDetails object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create userCredentialUsageDetails
Namespace: microsoft.graph

Create a new [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) object.

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
POST /reports/userCredentialUsageDetails
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) object.

The following table shows the properties that are required when you create the [userCredentialUsageDetails](../resources/usercredentialusagedetails.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|feature|featureType|**TODO: Add Description**. Possible values are: `registration`, `reset`, `unknownFutureValue`.|
|userPrincipalName|String|**TODO: Add Description**|
|userDisplayName|String|**TODO: Add Description**|
|isSuccess|Boolean|**TODO: Add Description**|
|authMethod|usageAuthMethod|**TODO: Add Description**. Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion`, `appNotification`, `appCode`, `alternateMobileCall`, `fido`, `appPassword`, `unknownFutureValue`.|
|failureReason|String|**TODO: Add Description**|
|eventDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_usercredentialusagedetails_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/reports/userCredentialUsageDetails
Content-Type: application/json
Content-length: 284

{
  "@odata.type": "#microsoft.graph.userCredentialUsageDetails",
  "feature": "String",
  "userPrincipalName": "String",
  "userDisplayName": "String",
  "isSuccess": "Boolean",
  "authMethod": "String",
  "failureReason": "String",
  "eventDateTime": "String (timestamp)"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.usercredentialusagedetails"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.userCredentialUsageDetails",
  "id": "e5d790f2-90f2-e5d7-f290-d7e5f290d7e5",
  "feature": "String",
  "userPrincipalName": "String",
  "userDisplayName": "String",
  "isSuccess": "Boolean",
  "authMethod": "String",
  "failureReason": "String",
  "eventDateTime": "String (timestamp)"
}
```

