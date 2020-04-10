---
title: "Add userExperienceAnalyticsBaselines"
description: "Add userExperienceAnalyticsBaselines by posting to the userExperienceAnalyticsBaselines collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add userExperienceAnalyticsBaselines

Namespace: microsoft.graph

Add userExperienceAnalyticsBaselines by posting to the userExperienceAnalyticsBaselines collection.

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
POST /deviceManagement/userExperienceAnalyticsBaselines/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_userexperienceanalyticsbaseline_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines
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
  "truncated": true,
  "@odata.type": "microsoft.graph.userexperienceanalyticsbaseline"
}
-->
``` http
HTTP/1.1 201 Created
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

