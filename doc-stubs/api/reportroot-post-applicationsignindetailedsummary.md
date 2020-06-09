---
title: "Create applicationSignInDetailedSummary"
description: "Create a new applicationSignInDetailedSummary object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create applicationSignInDetailedSummary
Namespace: microsoft.graph

Create a new applicationSignInDetailedSummary object.

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
POST /reports/applicationSignInDetailedSummary
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object.

The following table shows the properties that are required when you create the [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|appId|String|**TODO: Add Description**|
|appDisplayName|String|**TODO: Add Description**|
|status|[signInStatus](../resources/signinstatus.md)|**TODO: Add Description**|
|signInCount|Int64|**TODO: Add Description**|
|aggregatedEventDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_applicationsignindetailedsummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/reports/applicationSignInDetailedSummary
Content-Type: application/json
Content-length: 280

{
  "@odata.type": "#microsoft.graph.applicationSignInDetailedSummary",
  "appId": "String",
  "appDisplayName": "String",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus"
  },
  "signInCount": "Integer",
  "aggregatedEventDateTime": "String (timestamp)"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationsignindetailedsummary"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.applicationSignInDetailedSummary",
  "id": "286b1c07-1c07-286b-071c-6b28071c6b28",
  "appId": "String",
  "appDisplayName": "String",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus"
  },
  "signInCount": "Integer",
  "aggregatedEventDateTime": "String (timestamp)"
}
```

