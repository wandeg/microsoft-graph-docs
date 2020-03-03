---
title: "Update credentialUserRegistrationCount"
description: "Update the properties of a credentialUserRegistrationCount object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update credentialUserRegistrationCount

Update the properties of a [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) object.

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
PATCH ** Entity URI for microsoft.graph.credentialUserRegistrationCount not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [credentialUserRegistrationCount](../resources/credentialUserRegistrationCount.md) object.

The following table shows the properties that are required when you create the [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|totalUserCount|Int64||
|userRegistrationCounts|[userRegistrationCount](../resources/userRegistrationCount.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_credentialuserregistrationcount"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.credentialUserRegistrationCount not found
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.credentialUserRegistrationCount",
  "totalUserCount": 14,
  "userRegistrationCounts": [
    {
      "@odata.type": "microsoft.graph.userRegistrationCount",
      "registrationStatus": "String",
      "registrationCount": 1
    }
  ]
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
Content-Length: 330

{
  "@odata.type": "#microsoft.graph.credentialUserRegistrationCount",
  "id": "32a539a1-39a1-32a5-a139-a532a139a532",
  "totalUserCount": 14,
  "userRegistrationCounts": [
    {
      "@odata.type": "microsoft.graph.userRegistrationCount",
      "registrationStatus": "String",
      "registrationCount": 1
    }
  ]
}
```

