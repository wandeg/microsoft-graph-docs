---
title: "androidManagedStoreAccountEnterpriseSettings resource type"
description: "Enterprise settings for an Android managed store account."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# androidManagedStoreAccountEnterpriseSettings resource type


Namespace: microsoft.graph

Enterprise settings for an Android managed store account.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get androidManagedStoreAccountEnterpriseSettings](../api/androidmanagedstoreaccountenterprisesettings-get.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/androidmanagedstoreaccountenterprisesettings.md)|Read the properties and relationships of an [androidManagedStoreAccountEnterpriseSettings](../resources/androidmanagedstoreaccountenterprisesettings.md) object.|
|[Update androidManagedStoreAccountEnterpriseSettings](../api/androidmanagedstoreaccountenterprisesettings-update.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/androidmanagedstoreaccountenterprisesettings.md)|Update the properties of an [androidManagedStoreAccountEnterpriseSettings](../resources/androidmanagedstoreaccountenterprisesettings.md) object.|
|[approveApps](../api/androidmanagedstoreaccountenterprisesettings-approveapps.md)|None|**TODO: Add Description**|
|[requestSignupUrl](../api/androidmanagedstoreaccountenterprisesettings-requestsignupurl.md)|String|**TODO: Add Description**|
|[completeSignup](../api/androidmanagedstoreaccountenterprisesettings-completesignup.md)|None|**TODO: Add Description**|
|[syncApps](../api/androidmanagedstoreaccountenterprisesettings-syncapps.md)|None|**TODO: Add Description**|
|[unbind](../api/androidmanagedstoreaccountenterprisesettings-unbind.md)|None|**TODO: Add Description**|
|[createGooglePlayWebToken](../api/androidmanagedstoreaccountenterprisesettings-creategoogleplaywebtoken.md)|String|**TODO: Add Description**|
|[setAndroidDeviceOwnerFullyManagedEnrollmentState](../api/androidmanagedstoreaccountenterprisesettings-setandroiddeviceownerfullymanagedenrollmentstate.md)|None|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|androidDeviceOwnerFullyManagedEnrollmentEnabled|Boolean|Company codes for AndroidManagedStoreAccountEnterpriseSettings|
|bindStatus|androidManagedStoreAccountBindStatus|Bind status of the tenant with the Google EMM API. Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|companyCodes|[androidEnrollmentCompanyCode](../resources/androidenrollmentcompanycode.md) collection|Company codes for AndroidManagedStoreAccountEnterpriseSettings|
|deviceOwnerManagementEnabled|Boolean|Indicates if this account is flighting for Android Device Owner Management with CloudDPC.|
|enrollmentTarget|androidManagedStoreAccountEnrollmentTarget|Indicates which users can enroll devices in Android Enterprise device management. Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastAppSyncDateTime|DateTimeOffset|Last completion time for app sync|
|lastAppSyncStatus|androidManagedStoreAccountAppSyncStatus|Last application sync result. Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
|lastModifiedDateTime|DateTimeOffset|Last modification time for Android enterprise settings|
|ownerOrganizationName|String|Organization name used when onboarding Android Enterprise|
|ownerUserPrincipalName|String|Owner UPN that created the enterprise|
|targetGroupIds|String collection|Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
  "id": "String (identifier)",
  "bindStatus": "String",
  "lastAppSyncDateTime": "String (timestamp)",
  "lastAppSyncStatus": "String",
  "ownerUserPrincipalName": "String",
  "ownerOrganizationName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "enrollmentTarget": "String",
  "targetGroupIds": [
    "String"
  ],
  "deviceOwnerManagementEnabled": true,
  "companyCodes": [
    {
      "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode"
    }
  ],
  "androidDeviceOwnerFullyManagedEnrollmentEnabled": true
}
```

