# Optical Character Recognition

## Overview

Custom directive based on cordova to take pictures using the camera and convert the text in the picture to string. It can be used only on mobiles. If you want to use this add **n-ocr** custom directive to any component.

## Usage

This directive is intended to be added to any component. Once added any click event on the component will trigger the following function :-

* The camera on the mobile device will open.
* User is provided the option to take a picture.
* Once a picture is taken, all the text is converted into string and returned.

### How to use

1. Drag and drop any component and then add the following key-value pairs using the "New property : Attribute" section of the HTML page. Note :- If the value field is missing then leave it empty. If an input needs to be added to the value field, click the slide-toggle button; this makes the value field editable.
   1. Add the directive as an attribute.
      * key : n-ocr
      * Leave the value field empty
      * Click the ADD button
   2. Provide the options that the directive will use.
      * key : \[ocrOptions\] 
      * value : `{quality:100, correctOrientation: true, uriOrBase:0, returnType:1}`
      * Click the ADD button
   3. Input the action that occurs if the directive successfully completed its functionality.
      * key : \(onsuccess\)  
      * value : `success($event)`
      * Click the ADD button
      * Then is TS file add the following function `success($event){console.log($event)}`
   4. Input the action that occurs if the directive failed to complete its functionality.
      * key : \(onerror\)  
      * value : `error($event)`
      * Click the ADD button
      * Then is TS file add the following function `error($event){console.log($event)}`
2. The `console.log($event)` line inside the values of the \(onsuccess\) and \(onerror\) keys can be changed as per the developers requirement. 

   > Note :- `console.log($event)` displays the output \(which is $event\) of the directive for both success and error on a console which can be accessed by google chrome or safari.

## Support

* **Devices:** Android, iOS
* **Browsers:**  None
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

