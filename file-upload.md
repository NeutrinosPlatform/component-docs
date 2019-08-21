# File Upload

## Overview

File Upload is a button by clicking which the selected files can be uploaded.

## Usage

This component is used to provide an interface for the user to upload selected files \(such as scanned images, log files, etc.\).

### How to use

1. Drag and drop the **File Upload** component \(from palette component **Others** section\) to a location where it is needed in that page.
2. Double click on the component and set the required attributes.
3. Save the changes and run the page.

### Example

1. Create a page called **Profile**.
2. Drag and drop the **File Upload** component.
3. Double click the component. 
4. In the **Ts** file, create a property called **`uploadOptions`**and set its value as below.

   ```typescript
   uploadOptions = {"entityName":"users",
    "metadata":{"key":"user1@gmail.com"}
    }
   ```

5. Set the value of `uploadOptions` to _**uploadOptions**_.
6. Write a function in the Ts file as below:

   ```typescript
      onSuccess(){
           console.log("Succesfully uploaded!")
       }
   ```

7. Save the changes.
8. Open the address where the app is running.
9. A button with **choose file** as its value should appear.
10. Click the button and select a file to upload.
11. Click on the button again to upload.

## Associated Attributes

* **File Upload Label:** Specify the display name of the File Upload component.
* **Style:** It accepts a string value and affects different properties such as height, width, and color of the component based on the values provided. For example:  `background:orange;height:200px;`.
* **Class:** Used to point to a class in a style sheet. A class contains one or more style statements. Classes are created in the **Styles** editor by clicking  **Styles** in the editor menu. The `class` attribute accepts space separated class names which are defined as shown below:
* ```css
    .class1 {
        border-radius:10px;
        flex-basis:10%;
        height:100px;
    }
    .class2 {
        border-radius:10px;
        flex-basis:10%;
        height:100px;
    }
  ```
* **\[uploadOptions\]:** Specify the name of the object that is defined in the **Ts** file. The object is of type:

  ```typescript
    {"entityName": "user", "metadata":{"key": "aUniqueKey"}}
  ```

  Where ,

  * **`entityName`** is the name under which the files with same **`entityName`** are grouped.
  * **`key`** is used to uniquely identify the uploaded file.  

  Example:

  ```typescript
  uploadOptions = {"entityName":"users",
  "metadata":{"key":"sankarshanaj@gmail.com"}}
  ```

* **\(onsuccess\):** Specify the function \(that is defined in the **Ts** file\) name as argument which will be called when the upload is successful. Example:`onSuccess().`
* **\(onerror\):** Specify the function \(that is defined in the **Ts** file\) name as argument which will be called when an error occurs. Example: `onError().`
* Disabled: Specify if the component is disabled. Choose **`True`** or **`False`**.

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

