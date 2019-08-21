# Mini Fab Button

## Overview

A Mini FAB \(Floating Action Button\) is a standard material design component. It is shaped as a circle that represents a promoted action. When pressed, it may contain more related actions. Mini FAB, as its name suggests, floats over the content in a fixed position.

## Usage

Mini fab component can be used to contain more related actions.

### How to use

1. Drag and drop the **Mini FAB** component into a page container. 
2. Double click the component to display the list of attributes that can be used with it.
3. Fill the required attributes.
4. Save and run the page.

### Example

1. Drag and drop the **Mini FAB** component into a page container. 
2. Double click the component.
3. Input the component field\(s\) with the attribute value\(s\):   

    **`fabicon`** = _**decorate**_  

    **`Click`**= _**clickEvent\(\)**_  

4. Open the TS window by clicking![](../../../.gitbook/assets/image%20%281%29.png) in the editor window. Insert the following function:

   ```typescript
    clickEvent() { 
        alert("Button clicked!!!");
    }
   ```

5. Save and run the page.
6. When the page is loaded, a button named **decorate** will be displayed on the screen. The class `clickEvent()` will be executed when the button is pressed. On clicking the button, the alert message "Button clicked!!!" will be displayed.

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
* **fabicon:** Specifies the text or image to be shown on the button.
* **Color:** A drop-down list which accepts the color based on the angular material theme. You can choose between the following colors, or click the edit button to input the color of your choice:
  * Primary
  * Accent
  * Warn
* **\(click\):** Is an event that checks when the button is clicked.
* **Disabled**: Specifies whether the component is disabled or not. Choose `True` or `Fals`
* **Disable Ripple:** Specify whether ripple is disabled or not. Choose `True` or `False`.
* **type**: Design type of the button. For example- Raised button.
* **routerLink**: A link which navigates to a specified path.

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

