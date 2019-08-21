# Raised Button

## Overview

The Raised Button component represents a clickable button. The button appears raised compared to a normal button component.

## Usage

Raised Button allows the user to trigger an event. For example, searching for a query in a search engine, or to interact with dialog boxes to confirm action. It can be used to represent the importance of a specific functionality that is performed on click of this button.

### How to use

1. Drag and drop the **Raised Button** component. 
2. Double click the component to display the list of attributes that can be used with it.
3. Fill the required attributes.
4. Save and run the page.

### Example

1. Drag and drop the **Raised Button** component. 
2. Double click the component to display the list of attributes 
3. Input the component field\(s\) with the attribute value\(s\):

    **`buttonname`** = _**submit**_

    **`Click`** = _**clickEvent\(\)**_ 

4. Open the TS window by clicking![](../../../.gitbook/assets/image%20%281%29.png) in the editor window. Insert the following function:

   ```typescript
    clickEvent() { 
        alert("Button clicked!!!");
    }
   ```

5. Save and run the page.
6. When the page is loaded, a **submit** button will be displayed on the button and  `clickEvent()` runs when the button is pressed. On clicking the button, the alert message **Button clicked!!!** will be displayed.

## Associated Attributes

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
* **buttonname:** Specify the button name that is to be displayed on the screen.
* **Color:** A drop-down list which accepts the color based on the angular material theme. You can choose between the following colors, or click the edit button to input the color of your choice:
  * Primary
  * Accent
  * Warn
* **\(click\):** Is an event that runs when the button is clicked.
* **Disabled:** A Boolean value to specify whether the component is disabled or not. Choose `True` or `False`.
* **Disable Ripple:** A Boolean value to specify whether ripples are disabled. Toggle between `True` or `False`.
* **type**: Design type of the button. For example- Raised button.
* **routerLink**: A link which navigates to a specified path.

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

