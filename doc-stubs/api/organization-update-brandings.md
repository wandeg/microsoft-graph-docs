---
title: "Update brandings"
description: "Update the properties of a brandings object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update brandings
Namespace: microsoft.graph

Update the properties of a brandings object.

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
PATCH /organization/{organizationId}/brandings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [organizationalBranding](../resources/organizationalbranding.md) object.

The following table shows the properties that are required when you create the [organizationalBranding](../resources/organizationalbranding.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|backgroundColor|String|**TODO: Add Description**|
|backgroundImage|Stream|**TODO: Add Description**|
|bannerLogo|Stream|**TODO: Add Description**|
|locale|String|**TODO: Add Description**|
|signInPageText|String|**TODO: Add Description**|
|squareLogo|Stream|**TODO: Add Description**|
|usernameHintText|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [organizationalBranding](../resources/organizationalbranding.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_brandings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/brandings
Content-Type: application/json
Content-length: 269

{
  "@odata.type": "#microsoft.graph.organizationalBranding",
  "backgroundColor": "String",
  "backgroundImage": "Stream",
  "bannerLogo": "Stream",
  "locale": "String",
  "signInPageText": "String",
  "squareLogo": "Stream",
  "usernameHintText": "String"
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
  "@odata.type": "#microsoft.graph.organizationalBranding",
  "id": "f14009a6-09a6-f140-a609-40f1a60940f1",
  "backgroundColor": "String",
  "backgroundImage": "Stream",
  "bannerLogo": "Stream",
  "locale": "String",
  "signInPageText": "String",
  "squareLogo": "Stream",
  "usernameHintText": "String"
}
```

