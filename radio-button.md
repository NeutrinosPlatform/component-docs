# Radio Button

## Overview

A Radio Button is a button that can be either checked or unchecked. A user can tap the button to check or uncheck an attribute associated with that button. 

Use the Radio Group component to group a set of radio buttons. When radio buttons are placed inside a radio group, only one radio button in the group can be checked at any time. If a radio button is not placed in a group, they will all have the ability to be checked at the same time.

## Usage

Radio buttons are typically rendered as small circles, which are filled or highlighted when selected. It can be either checked or unchecked.

### How to use

1. Drag and drop a **Radio Button** to the page container. 
2. Double click the component to display the list of attributes that can be used with it.
3. Fill the attributes
4. Save and run the page.

### Example

1. Drag and drop a **Radio Button** to the page container. 
2. Double click the component to display the list of attributes
3. Input the component field\(s\) with the attribute value\(s\):  

    **`Checked`** = **oncheck\(\)**  

    **`Value`** = **option1**  

4. Open the TS window by clicking![](../../../.gitbook/assets/image%20%281%29.png) in the editor window. Insert the following function:

   ```typescript
    oncheck() { 
        alert("checkbox checked");
    }
   ```

5. Save and run the page.
6. When the page is loaded, the class **`oncheck()`**  event runs when the radio button is checked. On checking the radio button the alert message _**checkbox checked**_ will be displayed. The value attribute displays the text **option1** for the radio button.

## Associated Attributes

* **style:** Accepts a string value and affects different properties such as height, width, and color of the component based on the values provided. Example: `background:orange;height:200px;`.
* **class:** Used to point to a class in a style sheet. A class contains one or more style statements. Classes are created in the **Styles** editor by clicking  **Styles** in the editor menu. The **`class`** attribute accepts space separated class names. They are defined in the **`Style`** tab as shown below.
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
* **Radio Button Label:** Display name for the Radio Button.
* **Value:** It is the value given for the radio button. 
* **Required:** On page rendering, this field is used to check whether the radio button is a required field to be selected by the user, or not. 
* **label**: Is the label given for the radio button. 
* **id:** Is the unique ID for the radio button.
* **name:** Attribute used to group buttons for unique selection.
* **Checked:** A Boolean value that specifies whether the radio button is checked or not. Choose between `True` or `False`.
* **\(change\)**: Used to specify the event emitted when the group value changes. Change events are only emitted when the value changes due to user interaction with a radio button.
* **Labelposition:** Specifies whether the labels should appear after or before the radio-buttons. Defaults to **After**.
* **Disabled:** A Boolean value used to specify whether the radio button is disabled. Choose between `True` or `False`.
* **Disable Ripple:** A Boolean value used to specify if the ripple is disabled. Choose between `True` or`False`.
* **Color:** A drop-down list which accepts the color based on the angular material theme. You can choose between the following colors, or click the edit button to input the color of your choice:
  * Primary
  * Accent
  * Warn

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

