# Icon

## Overview

The Icon component represents an icon in the application. Icons are most effective as they improve visual interest and grab the user's attention. They guide users to navigate between pages.

### How to use

1. Drag and drop the **Icon** component into a page container.
2. Double click the component to display the list of attributes that can be used with it.
3. Fill the required attributes.
4. Save and run the page.

### Example

1. Drag and drop the **Icon** component into a page container.
2. Double click the component.
3. Input the component field\(s\) with the attribute value\(s\):   

    **`iconname`** = _**home**_  

   **`class`** = _**icon**_

4. Save and run the page.
5. When the page is loaded, a home icon will be displayed on the button. The class named `icon()` can be used to point to a class in the style sheet.

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
* **iconName:** Specify a name for the icon.
* **\[inine\]**:  A Boolean value to specify whether the icon should be inlined, automatically sizing the icon to match the font size of the element the icon is contained in. Choose **`True`** or **False**.
* **Color**: A drop-down list which accepts the color based on the angular material theme. You can choose between the following colors, or click the edit button to input the color of your choice:
  * Primary
  * Accent
  * Warn

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

