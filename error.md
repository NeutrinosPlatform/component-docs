# Error

## Overview

The Error component allows you to configure custom error messages to be displayed on screen when the error conditions are met.

### How to use

1. Drag and drop an **Error** component to the page container. 
2. Double click the component to display the list of attributes that can be used with it.
3. Fill the required attributes.
4. Save and run the page.

### Example

1. Drag and drop an **Input** component.
2. Open the Attributes window and enter u_**sername**_ for **`[(ngModel)]`** field.
3. Drag and drop an **Error** component to the page.
4. Click the Error component to open it's attributes window. 
5. Specify _**This field is required**_  as the error message in the **`Error Message`** field. 
6. Specify **`username.dirty`** as the error condition.
7. Save and run the page.
8. On page rendering, if you touch the Input component and do not specify a value, you will see a error message pop up.

## Associated Attributes

* **Error Label**: The Display name of the error.
* **style:** Accepts a string value that affects different properties of the Card such as height, width, and color, based on the values provided. For example: `background:orange:height:200px`.
* **class:** Used to point to a class in a style sheet.  Each class contains one or more style statements defined in the **Style** editor. The `Class` field accepts space separated class names such as `class1 class2` , where each class is defined in the Style editor as shown below:

  ```css
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

* **Error Message:** Enter the information to be displayed on the screen when the error is generated.
* **Error Condition:**  Specify the condition which defines an error.

#### Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

