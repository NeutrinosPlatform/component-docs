# Excel Sheet

## Overview

Custom directive to convert excel sheets into HTML. If you want to use this add **n-sheet** custom directive to any component.

## Usage

This directive is intended to be added to any component. Once added, on load of the component the following functionality will be triggered :-

* The n-sheet directive calls the n-sheet service which can be used seperately as well.
* Using the inputs \(explained below\) provide a http URL which is called where the Excel to HTML parser node resides within the B-Modelr.
* The inputs from the directive if valid will be used to convert the excel data which could either be an absolute file path or a file buffer into HTML ready to be inserted directly into any component on any page.

### How to use

1. For the directive to work you must first have your Excel Viewer Bmodeler Node setup. In your app folder find \flows\user-data\package.json and add the following dependecy `"node-red-exceltohtml" : "2.0.4"` then npm install within this folder and you are good to go. You might also have to setup your npm registry appropriately, plesae contact support to get help with this. 
2. Drag and drop any component and then add the following key-value pairs using the "New property : Attribute" section of the HTML page. Note :- If the value field is missing then leave it empty. If an input needs to be added to the value field, click the slide-toggle button; this makes the value field editable.
   1. Next add the directive as an attribute.
      * key : n-sheet
      * No value field
      * Click the ADD button
   2. Provide the inputs that the directive will use.
      * key : \[htmlContent\] 
      * value : \(Optional, used if sheetOptions not specified\) any html that will be directly populated to the component
      * key : \[sheetOptions\] 
      * value : \(Higher Preference input\) a variable that takes the following object as input from within the TS file. Replace type with value \(eg: boolean becomes true\)

        ```text
          {
              doAppend: boolean,                          // Optional  | Default value : false | If set to true does not clear the innerHTML of the component that the directive is being used within.
              url: 'string',                              // Mandatory | No Default value      | Required to call the HTTP request node that then calls the Excel to HTML parser node
              httpMethod: 'string',                       // Optional  | Default value : post  | If set to 'get' then the other sheetOptions can be provided within B modelr.
              preHttpRequestCallback: Promise/Boolean,    // Optional  | No Default value      | A Promise or a function that returns a boolean which runs right before url is called using the httpMethod. Will wait for the promise to complete. Can be used to check connectivity etc.  
              dataType: 'string',                         // Mandatory | No Default value      | Can take values 'file' or 'buffer', based on which the input sheetData has to be specified. For 'file', sheetData will be absolute filepath of the file on the system where B modelr is  running. For 'buffer', sheetData will be the file buffer of the file. This input need not be specified at the directive if it is specified in B modlr.
              sheetData: 'string',                        // Mandatory | No Default value      | THe absolute filepath or the file buffer based on the input dataType. This input need not be specified at the directive if it is specified in B modlr.
              retPure: boolean,                           // Not Valid | Default value : false | This variable returns each sheet as HTML in an array but cannot be used via the service or the directive, only via the B modelr.
              sheetIndices: Number Array[],               // Optional  | Default value : All   | A number array which is used to decide which sheets have to be rendered in the final output. Index of the sheets start from 0 till (total number of sheets - 1). If not specified all sheets will be returned.
              noParent: boolean                           // Optional  | Default value : false | If set to true, can be set to be viewed in full page views. Normal behaviour takes the height and width of the parent element
          }
        ```

      * Click the ADD button
   3. Input the action that occurs if the directive successfully completed its functionality.
      * key : \(onsuccess\)  
      * value : `success($event)`
      * Click the ADD button
      * Then is TS file add the following function `success($event){console.log($event)}`
      * The object returned on success contains the following values :-
        * In case of an exception a HTTP error object will be received.
        * In case of a success the excel rendered as HTML will be returned as a string. An array containing all the sheetnames and one with specified sheetnames \(if sheetIndices input was specified\) may also be returned if correct sheetOptions input was provided to the directive.
   4. Input the action that occurs if the directive failed to complete its functionality.
      * key : \(onerror\)  
      * value : `error($event)`
      * Click the ADD button
      * Then is TS file add the following function `error($event){console.log($event)}`
3. The `console.log($event)` line inside the values of the \(onsuccess\) and \(onerror\) keys can be changed as per the developers requirement. 

   > Note :- `console.log($event)` displays the output \(which is $event\) of the directive for both success and error on a console which can be accessed by google chrome or safari.

{% hint style="info" %}
When you use this directive, make sure you enable compression on the server to avoid performance issues as the HTML file that gets returned may be huge in size. You can check whether compression has been enabled by inspecting the response header **`Content-Encoding`**.
{% endhint %}

## Support

* **Devices:** Android, iOS
* **Browsers:**  Chrome, Firefox, Safari
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

