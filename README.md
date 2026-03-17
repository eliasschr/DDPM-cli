# Dell Display and Peripheral Manager 2.0 Command Line

This Documentation st based on two gist's:

https://gist.github.com/nebriv/cb934a3b702346c5988f2aba5ee39f0d
https://gist.github.com/eliasschr/7889a0e988f3e5778a2de14ab4c83313

Please use the issue feature incase an Updates messes the commands up (again). 
Otherwise, have fun. 

All available commands found in the CLI.

The full command looks like this:

```bash
/Applications/DDPM/DDPM.app/Contents/MacOS/DDPM /set -display=ActiveInputSource -value=USB-C
```

Write commands can be prefixed with `int:command` to specify which monitor to send the command to.

If you want to control your display through shortcuts, you can create a `.command` script and put it on your Desktop or in Stream Deck. Example:

```bash
#! /bin/bash
clear
/Applications/DDPM/DDPM.app/Contents/MacOS/DDPM /set -display=ActiveInputSource -value=USB-C
exit
```

Everything was tested on a Dell U4924DW and MacBook Pro running macOS 15.6.

- DDPM Version: `2.0.0.0018`
- Dell U4924DW Firmware Version: `M2B105`

> Quick info: These commands need admin access to run and cannot be executed by a normal user. If you've found any solutions to this issue, contributions are very welcome.

## Table of Contents
- [Monitor, App & Webcam Commands](#monitor-app--webcam-commands)
  - [Display Commands](#display-commands)
  - [App Commands](#app-commands)
  - [Webcam Commands](#webcam-commands)

# Monitor, App & Webcam Commands

## Display Commands

- [AutocolorPreset](#autocolorpreset)
- [ChangeMonitorID](#changemonitorid)
- [MonitorCount](#monitorcount)
- [ColorPreset](#colorpreset)
- [FWVersion](#fwversion)
- [BrightnessLevel](#brightnesslevel)
- [ContrastLevel](#contrastlevel)
- [ActiveInputSource](#activeinputsource)
- [SubInput](#subinput)
- [SwapVideo](#swapvideo)
- [SwapUSB](#swapusb)
- [PxPZoom](#pxpzoom)
- [RestoreFactoryDefaults](#restorefactorydefaults)
- [RestoreLevelDefaults](#restoreleveldefaults)
- [RestoreColorDefaults](#restorecolordefaults)
- [PowerSetting](#powersetting)
- [OSDLanguage](#osdlanguage)
- [OSDAccess](#osdaccess)
- [SpeakerVolume](#speakervolume)
- [Resolution](#resolution)
- [RefreshRate](#refreshrate)
- [EasyArrangeLayout](#easyarrangelayout)
- [Orientation](#orientation)
- [AllResolutionRefreshRate](#allresolutionrefreshrate)
- [CurrentResolutionRefreshRate](#currentresolutionrefreshrate)
- [AutoColorTemp](#autocolortemp)
- [PxP](#pxp)
- [FirmwareUpdate](#firmwareupdate)

### AutocolorPreset
**Set**

Value: On / Off

```bash
/set -display=AutoColorPreset -value=<example>
```

**Get**

```bash
/get -display=AutoColorPreset
```

### ChangeMonitorID
**Set**

Value: 0-100

```bash
/set -display=ChangeMonitorId -value=<example>
```

**Get**

*Not supported*

### MonitorCount
**Set**

*Not supported*

**Get**

```bash
/get -display=MonitorCount
```

### ColorPreset
**Set**

Value: standard, movie, game

```bash
/set -display=ColorPreset -value=<example>
```

**Get**

```bash
/get -display=ColorPreset
```

### FWVersion
**Set**

*Not supported*

**Get**

```bash
/get -display=FWVersion
```

### BrightnessLevel
**Set**

Value: 0-100

```bash
/set -display=BrightnessLevel -value=<example>
```

**Get**

Value: 0-100

```bash
/get -display=BrightnessLevel
```

### ContrastLevel
**Set**

Value: 0-100

```bash
/set -display=ContrastLevel -value=<example>
```

**Get**

Value: 0-100

```bash
/get -display=ContrastLevel
```

### ActiveInputSource
**Set**

Value: HDMI1, HDMI2, DP, USB-C

```bash
/set -display=ActiveInputSource -value=<example>
```

**Get**

Value: HDMI1, HDMI2, DP, USB-C

```bash
/get -display=ActiveInputSource
```

### SubInput
**Set**

Value: HDMI1, HDMI2, DP, USB-C

```bash
/set -display=SubInput -value=<example>
```

**Get**

Value: HDMI1, HDMI2, DP, USB-C

```bash
/get -display=SubInput
```

### SwapVideo
**Set**

Value: HDMI1, HDMI2, DP, USB-C

```bash
/set -display=SwapVideo -value=<example>
```

**Get**

*Not supported*

### SwapUSB
**Set**

```bash
/set display=SwapUSB
```

**Get**

*Not supported*

### PxPZoom
**Set**

Value: 0-∞?

```bash
/set -display=PxPZoom -value=<example>
```

**Get**

*Not supported*

### RestoreFactoryDefaults
**Set**

```bash
/set -display=RestoreFactoryDefaults
```

**Get**

*Not supported*

### RestoreLevelDefaults
**Set**

```bash
/set -display=RestoreLevelDefaults
```

**Get**

*Not supported*

### RestoreColorDefaults
**Set**

```bash
/set -display=RestoreColorDefaults
```

**Get**

*Not supported*

### PowerSetting
**Set**

Value: On / Off / Standby

```bash
/set -display=PowerSetting -value=<example>
```

**Get**

Value: On / Off / Standby

```bash
/get -display=PowerSetting
```

### OSDLanguage
**Set**

Value: english, german, …

```bash
/set -display=OSDLanguage -value=<example>
```

**Get**

Value: english, german, …

```bash
/get -display=OSDLanguage
```

### OSDAccess
**Set**

Value: OSDUnlock, OSDLock

```bash
/set -display=OSDAccess -value=<example>
```

**Get**

Value: OSDUnlock, OSDLock

```bash
/get -display=OSDAccess
```

### SpeakerVolume
**Set**

Value: 0-100

```bash
/set -display=SpeakerVolume -value=<example>
```

**Get**

Value: 0-100

```bash
/get -display=SpeakerVolume
```

### Resolution
**Set**

Value: 5120x1440

```bash
/set -display=Resolution -value=<example>
```

### RefreshRate
**Set**

Value: 30hz, 60hz

```bash
/set -display=RefreshRate -value=<example>
```

### EasyArrangeLayout
**Set**

```bash
/set -display=EasyArrangeLayout -value=<example>
```

**Get**

```bash
/get -display=EasyArrangeLayout
```

### Orientation
**Set**

Value: landscape / unknown

```bash
/set -display=Orientation -value=<example>
```

**Get**

```bash
/get -display=Orientation
```

### AllResolutionRefreshRate
**Get**

Value: Look at Chart

```bash
/get -display=AllResolutionRefreshRate
```

### CurrentResolutionRefreshRate
**Get**

```bash
/get -display=CurrentResolutionRefreshRate
```

### AutoColorTemp
**Set**

Value: On / Off

```bash
/set -display=AutoColorTemp -value=<example>
```

**Get**

```bash
/get -display=AutoColorTemp
```

### PxP
**Set**

Value: Off; PiP; PiP-Large; pbp-2h-fill; pbp-2h-2674; pbp-2h-7426;

```bash
/set -display=PxP -value=<example>
```

### FirmwareUpdate
**Set**

Value: unknown

```bash
/set -display=FirmwareUpdate -value=<example>
```

**Get**

Value: unknown

```bash
/get -display=FirmwareUpdate
```

## App Commands

- [Update](#update)
- [UpdateSourceLocation](#updatesourcelocation)
- [FirmwareUpdate](#firmwareupdate-1)
- [UpdateAccess](#updateaccess)
- [ScreenNotification](#screennotification)
- [ConnectedDevices](#connecteddevices)
- [DeviceData](#devicedata)
- [DeviceConfiguration](#deviceconfiguration)
- [DiagnosticsReport](#diagnosticsreport)
- [Rescan](#rescan)
- [InAppUpdate](#inappupdate)

### Update
**Set**

```bash
/set -app=Update
```

**Get**

*Not supported*

### UpdateSourceLocation
**Set**

Value: unknown

```bash
/set -app=UpdateSourceLocation -value=<example>
```

**Get**

```bash
/get -app=UpdateSourceLocation
```

### FirmwareUpdate
**Set**

Value: unknown

```bash
/set -app=FirmwareUpdate -value=<example>
```

**Get**

```bash
/get -app=FirmwareUpdate
```

### UpdateAccess
**Set**

Value: unknown

```bash
/set -app=UpdateAccess -value=<example>
```

**Get**

```bash
/get -app=UpdateAccess
```

### ScreenNotification
**Set**

Value: On / Off

```bash
/set -app=ScreenNotification -value=<example>
```

**Get**

```bash
/get -app=ScreenNotification
```

### ConnectedDevices
**Get**

```bash
/get -app=ConnectedDevices
```

### DeviceData
**Get**

```bash
/get -app=DeviceData
```

### DeviceConfiguration
**Set**

Value: unknown

```bash
/set -app=DeviceConfiguration -value=<example>
```

**Get**

Value: unknown

```bash
/get -app=DeviceConfiguration
```

### DiagnosticsReport
**Get**

```bash
/get -app=DiagnosticsReport
```

### Rescan
**Set**

Value: unknown

```bash
/set -app=Rescan -value=<example>
```

**Get**

```bash
/get -app=Rescan
```

### InAppUpdate
**Set**

Value: unknown

```bash
/set -app=InAppUpdate -value=<example>
```

**Get**

```bash
/get -app=InAppUpdate
```

## Webcam Commands

- [FWVersion](#fwversion-1)
- [FieldOfView](#fieldofview)
- [hdr](#hdr)
- [AntiFlicker](#antiflicker)
- [MicSwitch](#micswitch)
- [AIAutoFraming](#aiautoframing)

### FWVersion
**Set**

Value: untested

```bash
/set -Webcam=FWVersion -value=<example>
```

**Get**

Value: untested

```bash
/get -Webcam=FWVersion
```

### FieldOfView
**Set**

Value: untested

```bash
/set -Webcam=FieldOfView -value=<example>
```

**Get**

Value: untested

```bash
/get -Webcam=FieldOfView
```

### hdr
**Set**

Value: untested

```bash
/set -Webcam=hdr -value=<example>
```

**Get**

Value: untested

```bash
/get -Webcam=hdr
```

### AntiFlicker
**Set**

Value: untested

```bash
/set -Webcam=AntiFlicker -value=<example>
```

**Get**

Value: untested

```bash
/get -Webcam=AntiFlicker
```

### MicSwitch
**Set**

Value: untested

```bash
/set -Webcam=MicSwitch -value=<example>
```

**Get**

Value: untested

```bash
/get -Webcam=MicSwitch
```

### AIAutoFraming
**Set**

Value: untested

```bash
/set -Webcam=AIAutoFraming -value=<example>
```

**Get**

Value: untested

```bash
/get -Webcam=AIAutoFraming
```
