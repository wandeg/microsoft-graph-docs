---
title: "Update termsAndConditionsAcceptanceStatus"
description: "Update the properties of a termsAndConditionsAcceptanceStatus object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update termsAndConditionsAcceptanceStatus

Namespace: microsoft.graph

Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) object.

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
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) object.

The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userDisplayName|String||
|acceptedVersion|Int32||
|acceptedDateTime|DateTimeOffset||
|userPrincipalName|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_termsandconditionsacceptancestatus"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 264

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:06.7425918+03:00",
  "userPrincipalName": "User Principal Name value"
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
Content-Length: 313

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "767e7a6f-7a6f-767e-6f7a-7e766f7a7e76",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:06.7425918+03:00",
  "userPrincipalName": "User Principal Name value"
}
```

