﻿# Get windows10GeneralConfiguration

> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.

Read properties and relationships of the [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) object.
## Prerequisites
One of the following **scopes** is required to execute this API:

*DeviceManagementApps.ReadWrite.All; DeviceManagementConfiguration.ReadWrite.All; DeviceManagementConfiguration.Read.All*
## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceConfigurationAssignments/{deviceConfigurationAssignmentsId}/deviceConfiguration/
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/
```

## Optional query parameters
This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.
## Request headers
|Header|Value|
|---|---|
|Authorization|Bearer &lt;token&gt; Required.|
|Accept|application/json|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) object in the response body.

## Example
### Request
Here is an example of the request.
```http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 6047

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
    "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "accountsBlockAddingNonMicrosoftAccountEmail": true,
    "antiTheftModeBlocked": true,
    "automaticUpdateMode": "notifyDownload",
    "automaticUpdateSchedule": "everyday",
    "automaticUpdateTime": "11:58:32.2970000",
    "bluetoothBlocked": true,
    "bluetoothBlockAdvertising": true,
    "bluetoothBlockDiscoverableMode": true,
    "cameraBlocked": true,
    "cellularBlockDataWhenRoaming": true,
    "cellularBlockVpn": true,
    "cellularBlockVpnWhenRoaming": true,
    "certificatesBlockManualRootCertificateInstallation": true,
    "copyPasteBlocked": true,
    "cortanaBlocked": true,
    "defenderBlockEndUserAccess": true,
    "defenderDaysBeforeDeletingQuarantinedMalware": 12,
    "defenderSystemScanSchedule": "everyday",
    "defenderFilesAndFoldersToExclude": [
      "Defender Files And Folders To Exclude value"
    ],
    "defenderFileExtensionsToExclude": [
      "Defender File Extensions To Exclude value"
    ],
    "defenderScanMaxCpu": 2,
    "defenderMonitorFileActivity": "disable",
    "defenderProcessesToExclude": [
      "Defender Processes To Exclude value"
    ],
    "defenderPromptForSampleSubmission": "alwaysPrompt",
    "defenderRequireBehaviorMonitoring": true,
    "defenderRequireCloudProtection": true,
    "defenderRequireNetworkInspectionSystem": true,
    "defenderRequireRealTimeMonitoring": true,
    "defenderScanArchiveFiles": true,
    "defenderScanDownloads": true,
    "defenderScanNetworkFiles": true,
    "defenderScanIncomingMail": true,
    "defenderScanMappedNetworkDrivesDuringFullScan": true,
    "defenderScanRemovableDrivesDuringFullScan": true,
    "defenderScanScriptsLoadedInInternetExplorer": true,
    "defenderSignatureUpdateIntervalInHours": 6,
    "defenderScanType": "disabled",
    "defenderScheduledScanTime": "11:59:10.9990000",
    "defenderScheduledQuickScanTime": "11:58:49.3840000",
    "deviceManagementBlockFactoryResetOnMobile": true,
    "deviceManagementBlockManualUnenroll": true,
    "diagnosticsDataSubmissionMode": "none",
    "oneDriveDisableFileSync": true,
    "edgeBlockAutofill": true,
    "edgeBlocked": true,
    "edgeCookiePolicy": "allow",
    "edgeBlockDeveloperTools": true,
    "edgeBlockSendingDoNotTrackHeader": true,
    "edgeBlockExtensions": true,
    "edgeBlockInPrivateBrowsing": true,
    "edgeBlockJavaScript": true,
    "edgeBlockPasswordManager": true,
    "safeSearchFilter": "strict",
    "edgeBlockPopups": true,
    "edgeBlockSearchSuggestions": true,
    "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
    "edgeRequireSmartScreen": true,
    "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
    "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
    "edgeSearchEngine": {
      "@odata.type": "microsoft.graph.edgeSearchEngineBase"
    },
    "edgeHomepageUrls": [
      "Edge Homepage Urls value"
    ],
    "edgeBlockAccessToAboutFlags": true,
    "smartScreenBlockPromptOverride": true,
    "smartScreenBlockPromptOverrideForFiles": true,
    "webRtcBlockLocalhostIpAddress": true,
    "internetSharingBlocked": true,
    "settingsBlockAddProvisioningPackage": true,
    "settingsBlockRemoveProvisioningPackage": true,
    "settingsBlockChangeSystemTime": true,
    "settingsBlockEditDeviceName": true,
    "settingsBlockChangeRegion": true,
    "settingsBlockChangeLanguage": true,
    "settingsBlockChangePowerSleep": true,
    "settingsBlockSettingsApp": true,
    "settingsBlockSystemPage": true,
    "settingsBlockDevicesPage": true,
    "settingsBlockNetworkInternetPage": true,
    "settingsBlockPersonalizationPage": true,
    "settingsBlockAccountsPage": true,
    "settingsBlockTimeLanguagePage": true,
    "settingsBlockEaseOfAccessPage": true,
    "settingsBlockPrivacyPage": true,
    "settingsBlockUpdateSecurityPage": true,
    "locationServicesBlocked": true,
    "lockScreenBlockActionCenterNotifications": true,
    "microsoftAccountBlocked": true,
    "microsoftAccountBlockSettingsSync": true,
    "nfcBlocked": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordMinimumCharacterSetCount": 0,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordRequired": true,
    "passwordRequireWhenResumeFromIdleState": true,
    "passwordRequiredType": "alphanumeric",
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "prereleaseFeatures": "settingsOnly",
    "resetProtectionModeBlocked": true,
    "screenCaptureBlocked": true,
    "storageBlockRemovableStorage": true,
    "storageRequireMobileDeviceEncryption": true,
    "usbBlocked": true,
    "voiceRecordingBlocked": true,
    "wiFiBlockAutomaticConnectHotspots": true,
    "wiFiBlocked": true,
    "wiFiBlockManualConfiguration": true,
    "windowsStoreBlocked": true,
    "appsAllowTrustedAppsSideloading": "blocked",
    "windowsStoreBlockAutoUpdate": true,
    "developerUnlockSetting": "blocked",
    "sharedUserAppDataAllowed": true,
    "appsBlockWindowsStoreOriginatedApps": true,
    "windowsStoreEnablePrivateStoreOnly": true,
    "storageRestrictAppDataToSystemVolume": true,
    "storageRestrictAppInstallToSystemVolume": true,
    "gameDvrBlocked": true,
    "experienceBlockWindowsSpotlight": true,
    "experienceBlockWindowsTips": true,
    "experienceBlockConsumerSpecificFeatures": true,
    "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
    "startMenuMode": "fullScreen",
    "logonBlockFastUserSwitching": true,
    "startBlockUnpinningAppsFromTaskbar": true
  }
}
```



