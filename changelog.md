# Changelog

## 1.4.18296.4 \(Preview\) - 2018-10-23

### Added

* Added Launcher component for Windows in XPlat.Device.Launcher
* Added RequestCodeHelper for aiding with Android intents to XPlat.Core
* Implemented Properties properties on StorageFile and StorageFolder for Windows in XPlat.Storage

### Changed

* [Issue 26 - Port to .NET Standard](https://github.com/jamesmcroft/XPlat-Windows-APIs/issues/26)
  * All projects have been moved to .NET Standard 1.4 and use multi-targeting to provide platform specific code.
  * XPlat.Storage library has split out into XPlat.Storage and XPlat.Storage.Pickers libraries to be inline with Windows SDK
  * XPlat.Media library has been renamed to XPlat.Media.Capture to be inline with Windows SDK
  * Launcher class in XPlat.Device.Launcher is no longer static and implements an interface for better cross-platform-ability 
  * NSDate and NSObject extensions for iOS moved to XPlat.Core
* Marked the ParseHelper class as **obsolete** with plan to remove in a future release. 

### Fixed

* [Issue 29 - CameraCaptureUI doesn't inform the user that they cancelled permissions](https://github.com/jamesmcroft/XPlat-Windows-APIs/issues/29)
  * Fixed issue with the CameraCaptureUI class for Android where denying permissions would not allow the developer to handle this scenario.
* [Issue 32 - Launcher API for Android doesn't launch files from local storage](https://github.com/jamesmcroft/XPlat-Windows-APIs/issues/32)
  * Fixed issue with the Launcher class for Android where attempting a launch on a StorageFile would result in the external application not being able to access the file.
* Fixed issue with the CoreDispatcher class for Windows would sometimes not run the action provided due to the dispatcher already having thread access.

## 1.3.18257.3 - 2018-09-14

### Fixed

* [Issue 25 - System.IO.File.Exists and System.IO.Directory.Exists don't behave as expected on UWP](https://github.com/jamesmcroft/XPlat-Windows-APIs/issues/25)
  * Removed the System.IO.File.Exists and System.IO.Directory.Exists method calls from the UWP StorageFile and StorageFolder classes to prevent issues with accessing data due to limitation in Windows where data is usually isolated to the app storage.



