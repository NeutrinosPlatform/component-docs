# Button Toggle

## Overview

A Button Toggle component is used to toggle between on and off. When the button is clicked, the button gets activated. When the button is clicked again, the button gets deactivated.

## Usage

A Button Toggle is a specialized control which has the ability to be selected. It is used to activate button on/off.

### How to use

1. Drag and drop a **Button Toggle** component. 
2. Double click the component to display the list of attributes that can be used with it.
3. Fill the required attributes.
4. Save and run the page.

### Example

1. Input the component field\(s\) with the attribute value\(s\):  

    **`Class`** = _**toggle**_  

    **`buttonname`** = _**on/off**_

2. Save and run the page.
3. When the page is loaded, a toggle button will be displayed with the name **on/off**. The class **toggle** can be used to point the class in the style sheet. 

## Associated Attributes

* **style:** Accepts a string value and affects different properties such as height, width, and color of the component based on the values provided. Example: `background:orange;height:200px;`.
* **class:** Used to point to a class in a style sheet. A class contains one or more style statements. Classes are created in the **Styles** editor by clicking  **Styles** in the editor menu. The `class` attribute accepts space separated class names. They are defined in the **`Style`** tab as shown below.

```text
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

* **value:** Specify the value of the Button Toggle. **`MatButtonToggleGroup`** reads this value to assign its own value.
* **buttonname:** Specify the button name.
* **name:** Specify the name attribute for the underlying input element.
* **id:** Specify a unique ID for this toggle button.
* **Checked:** A Boolean value to specify whether the button is checked. Choose `True` or `False`.
* **\(change\):** The event emitted when the group value changes.
* **\(click\):** The event used to check whether the button is clicked or not.

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:**
  * Angular CLI version: 6.0.0 +
  * Cordova version: 7.1.0 +

