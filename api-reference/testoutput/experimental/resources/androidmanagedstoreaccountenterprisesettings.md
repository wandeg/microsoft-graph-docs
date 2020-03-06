---
title: "androidManagedStoreAccountEnterpriseSettings resource type"
description: "Enterprise settings for an Android managed store account."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# androidManagedStoreAccountEnterpriseSettings resource type


Namespace: microsoft.graph

Enterprise settings for an Android managed store account.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get androidManagedStoreAccountEnterpriseSettings](../api/androidmanagedstoreaccountenterprisesettings-get.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/androidmanagedstoreaccountenterprisesettings.md)|Read properties and relationships of the [androidManagedStoreAccountEnterpriseSettings](../resources/androidmanagedstoreaccountenterprisesettings.md) object.|
|[Update androidManagedStoreAccountEnterpriseSettings](../api/androidmanagedstoreaccountenterprisesettings-update.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/androidmanagedstoreaccountenterprisesettings.md)|Update the properties of a [androidManagedStoreAccountEnterpriseSettings](../resources/androidmanagedstoreaccountenterprisesettings.md) object.|
|[approveApps](../api/androidmanagedstoreaccountenterprisesettings-approveapps.md)|None||
|[requestSignupUrl](../api/androidmanagedstoreaccountenterprisesettings-requestsignupurl.md)|String||
|[completeSignup](../api/androidmanagedstoreaccountenterprisesettings-completesignup.md)|None||
|[syncApps](../api/androidmanagedstoreaccountenterprisesettings-syncapps.md)|None||
|[unbind](../api/androidmanagedstoreaccountenterprisesettings-unbind.md)|None||
|[createGooglePlayWebToken](../api/androidmanagedstoreaccountenterprisesettings-creategoogleplaywebtoken.md)|String||
|[setAndroidDeviceOwnerFullyManagedEnrollmentState](../api/androidmanagedstoreaccountenterprisesettings-setandroiddeviceownerfullymanagedenrollmentstate.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|androidDeviceOwnerFullyManagedEnrollmentEnabled|Boolean|Company codes for AndroidManagedStoreAccountEnterpriseSettings|
|bindStatus|Enumeration|Bind status of the tenant with the Google EMM API. Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|companyCodes|[androidEnrollmentCompanyCode](../resources/androidenrollmentcompanycode.md) collection|Company codes for AndroidManagedStoreAccountEnterpriseSettings|
|deviceOwnerManagementEnabled|Boolean|Indicates if this account is flighting for Android Device Owner Management with CloudDPC.|
|enrollmentTarget|Enumeration|Indicates which users can enroll devices in Android Enterprise device management. Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastAppSyncDateTime|DateTimeOffset|Last completion time for app sync|
|lastAppSyncStatus|Enumeration|Last application sync result. Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
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

