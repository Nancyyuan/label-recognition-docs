---
layout: default-layout
title: Dynamsoft Label Recognition C++ API Reference - Result
description: This is the result functions of Dynamsoft Label Recognition for C++ API Reference.
keywords: api reference, cpp
needAutoGenerateSidebar: false
---

# C++ API Reference - Result

| Method               | Description |
|----------------------|-------------|
  | [`GetAllDLRResults`](#getalldlrresults) | Gets all recognized results. |
  | [`FreeDLRResults`](#freedlrresults) | Frees memory allocated for recognized results. |

---

## GetAllDLRResults
Get all recognized results.

```cpp
int dynamsoft::dlr::CLabelRecognition::GetAllDLRResults (DLRResultArray** results)	
```   
   
#### Parameters
`[out] results`	Recognized results returned by last calling function [`RecognizeByBuffer`](recognizing.md#recognizebybuffer) / [`RecognizeByFile`](recognizing.md#recognizebyfile) / [`RecognizeBasedOnDBRResultByBuffer`](recognizing.md#recognizebasedondbrresultbybuffer) / [`RecognizeBasedOnDBRResultByFile`](recognizing.md#recognizebasedondbrresultbyfile). The results is allocated by SDK and should be freed by calling function [`FreeDLRResults`](#freedlrresults).

#### Return value
Returns error code (returns 0 if the function operates successfully).    
*You can call [`GetErrorString`](general.md#geterrorstring) to get detailed error message.*

#### Code Snippet
```cpp
CLabelRecognition* recognizer = new CLabelRecognition();
recognizer->InitLicense("t0260NwAAAHV***************");
DLRResultArray * results;
int errorCode = recognizer->RecognizeByFile("C:\\Program Files (x86)\\Dynamsoft\\{Version number}\\Images\\AllSupportedBarcodeTypes.tif", "");
recognizer->GetAllDLRResults(&results);
dynamsoft::dlr::CLabelRecognition::FreeDLRResults(&results);
delete recognizer;
```

&nbsp;

## FreeDLRResults
Free memory allocated for text results.

```cpp
static void dynamsoft::dlr::CLabelRecognition::FreeDLRResults (DLRResultArray ** results)	
```   
   
#### Parameters
`[in]	results` Recognized results.

#### Code Snippet
```cpp
CLabelRecognition* recognizer = new CLabelRecognition();
recognizer->InitLicense("t0260NwAAAHV***************");
DLRResultArray * results;
int errorCode = recognizer->RecognizeByFile("C:\\Program Files (x86)\\Dynamsoft\\{Version number}\\Images\\AllSupportedBarcodeTypes.tif", "");
recognizer->GetAllDLRResults(&results);
dynamsoft::dlr::CLabelRecognition::FreeDLRResults(&results);
delete recognizer;
```

&nbsp;
