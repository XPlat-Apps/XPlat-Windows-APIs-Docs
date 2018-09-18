# Changelog

## 1.4.18260.2 \(Preview\) - 2018-09-17

### Added

* Added Launcher component for Windows in XPlat.Devices.Launcher
* Added RequestCodeHelper for aiding with Android intents to XPlat.Core
* Implemented Properties properties on StorageFile and StorageFolder for Windows in XPlat.Storage

### Changed

* [Issue 26 - Port to .NET Standard](https://github.com/jamesmcroft/XPlat-Windows-APIs/issues/26)
  * All projects have been moved to .NET Standard 1.4 and use multi-targeting to provide platform specific code.
  * XPlat.Storage library has split out into XPlat.Storage and XPlat.Storage.Pickers libraries to be inline with Windows SDK
  * XPlat.Device.{x} libraries have been renamed to XPlat.Devices.{x}
    * This is a breaking change as namespaces have been updated to reflect changes.
  * XPlat.Media library has been renamed to XPlat.Media.Capture to be inline with Windows SDK
  * Launcher class in XPlat.Devices.Launcher is no longer static and implements an interface for better cross-platform-ability 
  * NSDate and NSObject extensions for iOS moved to XPlat.Core

### Removed

* ParseHelper class has been removed from XPlat.Core

### Fixed

* Fixed issue with the CoreDispatcher class for Windows would sometimes not run the action provided due to the dispatcher already having thread access.

## 1.3.18257.3 - 2018-09-14

### Fixed

* [Issue 25 - System.IO.File.Exists and System.IO.Directory.Exists don't behave as expected on UWP](https://github.com/jamesmcroft/XPlat-Windows-APIs/issues/25)
  * Removed the System.IO.File.Exists and System.IO.Directory.Exists method calls from the UWP StorageFile and StorageFolder classes to prevent issues with accessing data due to limitation in Windows where data is usually isolated to the app storage.



