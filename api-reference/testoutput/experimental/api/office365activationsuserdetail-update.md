---
title: "Update office365ActivationsUserDetail"
description: "Update the properties of a office365ActivationsUserDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update office365ActivationsUserDetail

Namespace: microsoft.graph

Update the properties of a [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) object.

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
PATCH ** Entity URI for microsoft.graph.office365ActivationsUserDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) object.

The following table shows the properties that are required when you create the [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|userPrincipalName|String||
|displayName|String||
|userActivationCounts|[userActivationCounts](../resources/useractivationcounts.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_office365activationsuserdetail"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.office365ActivationsUserDetail not found
Content-type: application/json
Content-length: 535

{
  "@odata.type": "#microsoft.graph.office365ActivationsUserDetail",
  "reportRefreshDate": "Date",
  "userPrincipalName": "User Principal Name value",
  "displayName": "Display Name value",
  "userActivationCounts": [
    {
      "@odata.type": "microsoft.graph.userActivationCounts",
      "productType": "Product Type value",
      "lastActivatedDate": "Date",
      "windows": 7,
      "mac": 3,
      "windows10Mobile": 15,
      "ios": 3,
      "android": 7,
      "activatedOnSharedComputer": true
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
Content-Length: 584

{
  "@odata.type": "#microsoft.graph.office365ActivationsUserDetail",
  "id": "6f7e8fa8-8fa8-6f7e-a88f-7e6fa88f7e6f",
  "reportRefreshDate": "Date",
  "userPrincipalName": "User Principal Name value",
  "displayName": "Display Name value",
  "userActivationCounts": [
    {
      "@odata.type": "microsoft.graph.userActivationCounts",
      "productType": "Product Type value",
      "lastActivatedDate": "Date",
      "windows": 7,
      "mac": 3,
      "windows10Mobile": 15,
      "ios": 3,
      "android": 7,
      "activatedOnSharedComputer": true
    }
  ]
}
```

