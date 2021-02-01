---
layout: default-layout
title: Dynamsoft Label Recognition .Net API Reference - Main Page
description: This is the main page of Dynamsoft Label Recognition for .Net API Reference.
keywords: api reference, .Net
needAutoGenerateSidebar: false
breadcrumbText: API Reference
---

# Dynamsoft Label Recognition - .Net API Reference

- [`LabelRecognition` Methods](#label-recognition-methods) 
- [Classes](#classes)  
- [Enumerations](#enumerations)
- [Error Code](#error-code)

## LabelRecognition Methods

### General
   
  | Method               | Description |
  |----------------------|-------------|
  | [`GetVersion`](label-recognition/general.md#getversion) | Returns the version number string for the SDK. |
   
&nbsp; 

### Initialization
  
  | Method               | Description |
  |----------------------|-------------|
  | [`LabelRecognition`](label-recognition/initialization.md#labelrecognition) | Constructor of `LabelRecognition` object.|
  | [`Dispose`](label-recognition/initialization.md#dispose) | Destroys an instance of `LabelRecognition` object.|   
  | [`InitLicense`](label-recognition/initialization.md#initlicense) | Sets the license and activates the SDK. |
  | [`InitLicenseFromLTS`](label-recognition/initialization.md#initlicensefromlts) | Initializes the label recognition license and connects to the specified server for online verification. |

&nbsp; 

### Settings

  | Method               | Description |
  |----------------------|-------------|
  | [`GetRuntimeSettings`](label-recognition/settings.md#getruntimesettings) | Gets the current settings and saves it into a struct. |
  | [`UpdateRuntimeSettings`](label-recognition/settings.md#updateruntimesettings) | Updates runtime settings with a given struct. |
  | [`ResetRuntimeSettings`](label-recognition/settings.md#resetruntimesettings) | Resets the runtime settings. |
  | [`AppendSettingsFromString`](label-recognition/settings.md#appendsettingsfromstring) | Appends LabelRecognitionParameter settings in a string to the SDK object. |
  | [`OutputSettingsToFile`](label-recognition/settings.md#outputsettingstofile) | Outputs LabelRecognitionParameter settings into a file (JSON file). |
  | [`ClearAppendedSettings`](label-recognition/settings.md#clearappendedsettings) | Clear all appended LabelRecognitionParameter settings in the SDK object. |
  | [`UpdateReferenceRegionFromBarcodeResults`](label-recognition/settings.md#updatereferenceregionfrombarcoderesults) | Updates reference region which is defined with source type DLR_LST_BARCODE. |
  | [`GetModeArgument`](label-recognition/settings.md#getmodeargument) | Get argument value for the specified mode parameter. |
  | [`SetModeArgument`](label-recognition/settings.md#setmodeargument) | Set argument value for the specified mode parameter. |

&nbsp; 
   
### Recognizing
   
  | Method               | Description |
  |----------------------|-------------|
  | [`RecognizeByBuffer`](label-recognition/recognizing.md#recognizebybuffer) | Recognizes text from memory buffer containing image pixels in defined format. |
  | [`RecognizeByFile`](label-recognition/recognizing.md#recognizebyfile) | Recognizes text from a specified image file. |
   
&nbsp; 

## [Class](class/index.md)
- [`DMLTSConnectionParameters`](class/dm-lts-connection-parameters.md)
- [`DLR_CharacterResult`](class/dlr-character-result.md)		
- [`DLR_Exception`](class/label-recognition-exception.md)	
- [`DLR_ImageData`](class/dlr-image-data.md)		
- [`DLR_LineResult`](class/dlr-line-Result.md)	
- [`DLR_Quadrilateral`](class/dlr-quadrilateral.md)	
- [`DLR_ReferenceRegion`](class/dlr-reference-region.md)	
- [`DLR_Result`](class/dlr-result.md)		
- [`DLR_RuntimeSettings`](class/dlr-runtime-settings.md)	

&nbsp; 

## [Enumerations]({{ site.enumerations }})
- [`EnumDLRImagePixelFormat`]({{ site.enumerations }}other-enums.html#enumdlrimagepixelformat)
- [`EnumDLRRegionPredetectionMode`]({{ site.enumerations }}parameter-mode-enums.html#enumdlrregionpredetectionmode)
- [`EnumDLRBinarizationMode`]({{ site.enumerations }}parameter-mode-enums.html#enumdlrbinarizationmode)
- [`EnumDLRGrayscaleTransformationMode`]({{ site.enumerations }}parameter-mode-enums.html#enumdlrgrayscaletransformationmode)
- [`EnumDMChargeWay`]({{ site.enumerations }}other-enums.html#enumdmchargeway)	
- [`EnumDMDeploymentType`]({{ site.enumerations }}other-enums.html#enumdmdeploymenttype)	
- [`EnumDMLicenseModule`]({{ site.enumerations }}other-enums.html#enumdmlicensemodule)	
- [`EnumDMUUIDGenerationMethod`]({{ site.enumerations }}other-enums.html#enumdmuuidgenerationmethod)	

&nbsp; 

## [Error Code]({{ site.enumerations }}error-code.html)
		