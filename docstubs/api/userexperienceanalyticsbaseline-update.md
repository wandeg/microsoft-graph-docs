---
title: "Update userExperienceAnalyticsBaseline"
description: "Update the properties of a userExperienceAnalyticsBaseline object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update userExperienceAnalyticsBaseline

Namespace: microsoft.graph

Update the properties of a [userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md) object.

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
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md) object.

The following table shows the properties that are required when you create the [userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|isBuiltIn|Boolean||
|createdDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_userexperienceanalyticsbaseline"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "displayName": "Display Name value",
  "isBuiltIn": true
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "id": "4af27402-7402-4af2-0274-f24a0274f24a",
  "displayName": "Display Name value",
  "isBuiltIn": true,
  "createdDateTime": "2016-12-31T23:58:51.3349474+00:00"
}
```

