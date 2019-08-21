# Button

## Overview

The Button component represents a clickable button, which can be used in forms, or anywhere in a document that needs simple, standard button functionality.

## Usage

A Button refers to any graphical control element that provides the user a simple way to trigger an event, like searching for a query in a search engine, or to interact with dialog boxes, like confirming an action.

### How to use

1. Drag and drop a Button component. 
2. Double click the component to display a list of attributes that can be used with it.
3. Fill the required attributes 
4. Save and run the page.

### Example

1. Input the component field\(s\) with the attribute value\(s\):  

    **`buttonname`** = _**submit**_  

    **`Click`** = _**clickEvent\(\)**_  

2. Open the TS window by clicking![](../../../.gitbook/assets/image%20%281%29.png) in the editor window. Insert the following function:

   ```typescript
    clickEvent() { 
        alert("Button clicked!!!");
    }
   ```

3. Save and run the page.
4. When the page is loaded, you will see a button named Submit, and when clicked, the `clickEvent()` class is executed. On clicking the button, the alert message **Button clicked!!!** will be displayed.

## Associated Attributes

* **style:** Accepts a string value and affects different properties such as height, width, and color of the component based on the values provided. Example: `background:orange;height:200px;`.
* **class:** Used to point to a class in a style sheet. A class contains one or more style statements. Classes are created in the **Styles** editor by clicking  **Styles** in the editor menu. The `class` attribute accepts space separated class names. They are defined in the "Style" tab as shown below.
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
* **Buttonname:** Specify the button name that is to be displayed on the screen.
* **Color:** A drop-down list which accepts the color based on the angular material theme. You can choose between the following colors, or click the edit button to input the color of your choice:
  * Primary
  * Accent
  * Warn
* **\(click\):** An event that runs when the button is clicked.
* **Disabled**: A Boolean value that specifies whether the component is disabled or not. Choose `True` or `False`.
* **Disable Ripple**: A Boolean value that specifies whether ripple is disabled or not. Choose `True` or `False`.
* **type**: Design type of the button. For example- Raised button.
* **routerLink**: A link which navigates to a specified path.

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

