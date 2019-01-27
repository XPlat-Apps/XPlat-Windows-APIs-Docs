# Changelog

## 1.5.19024.1 - 2019-01-25

### Added

* [#19](https://github.com/XPlat-Apps/XPlat-Windows-APIs/issues/19) - Added MessageDialog APIs to new XPlat.UI.Popups library
* [#36](https://github.com/XPlat-Apps/XPlat-Windows-APIs/issues/36) - Added Package APIs to new XPlat.ApplicationModel library
* [#41](https://github.com/XPlat-Apps/XPlat-Windows-APIs/issues/41) - Added Color API to new XPlat.UI library
* [#42](https://github.com/XPlat-Apps/XPlat-Windows-APIs/issues/42) - Added ColorHelper API to new XPlat.UI library
* [#43](https://github.com/XPlat-Apps/XPlat-Windows-APIs/issues/43) - Added Colors API to new XPlat.UI library
* [#40](https://github.com/XPlat-Apps/XPlat-Windows-APIs/issues/40) - Added AnalyticsInfo and AnalyticsVersionInfo APIs to new XPlat.Device.Profile library

### Changed

* Added [SourceLink](https://docs.microsoft.com/en-us/dotnet/standard/library-guidance/sourcelink) support to all project libraries

## 1.4.18299.4 - 2018-10-26

### Added

* Added Launcher component for Windows in XPlat.Device.Launcher
* Added RequestCodeHelper for aiding with Android intents to XPlat.Core
* Implemented Properties properties on StorageFile and StorageFolder for Windows in XPlat.Storage

### Changed

* [Issue 26 - Port to .NET Standard](https://github.com/XPlat-Apps/XPlat-Windows-APIs/issues/26)
  * All projects have been moved to .NET Standard 1.4 and use multi-targeting to provide platform specific code.
  * XPlat.Storage library has split out into XPlat.Storage and XPlat.Storage.Pickers libraries to be inline with Windows SDK
  * XPlat.Media library has been renamed to XPlat.Media.Capture to be inline with Windows SDK
  * Launcher class in XPlat.Device.Launcher is no longer static and implements an interface for better cross-platform-ability 
  * NSDate and NSObject extensions for iOS moved to XPlat.Core
* Marked the ParseHelper class as **obsolete** with plan to remove in a future release. 

### Fixed

* [Issue 29 - CameraCaptureUI doesn't inform the user that they cancelled permissions](https://github.com/XPlat-Apps/XPlat-Windows-APIs/issues/29)
  * Fixed issue with the CameraCaptureUI class for Android where denying permissions would not allow the developer to handle this scenario.
* [Issue 32 - Launcher API for Android doesn't launch files from local storage](https://github.com/XPlat-Apps/XPlat-Windows-APIs/issues/32)
  * Fixed issue with the Launcher class for Android where attempting a launch on a StorageFile would result in the external application not being able to access the file.
* Fixed issue with the CoreDispatcher class for Windows would sometimes not run the action provided due to the dispatcher already having thread access.

## 1.3.18257.3 - 2018-09-14

### Fixed

* [Issue 25 - System.IO.File.Exists and System.IO.Directory.Exists don't behave as expected on UWP](https://github.com/XPlat-Apps/XPlat-Windows-APIs/issues/25)
  * Removed the System.IO.File.Exists and System.IO.Directory.Exists method calls from the UWP StorageFile and StorageFolder classes to prevent issues with accessing data due to limitation in Windows where data is usually isolated to the app storage.



