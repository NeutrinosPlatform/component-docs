# Slide Toggle

## Overview

The Slide Toggle component is used to toggle between on/off. The toggle allows the user to change a setting between two states.

### How to use

1. Drag and drop the **Slide Toggle** component. 
2. Double click the component to display the list of attributes that can be used with it.
3. Fill the required attributes 
4. Save and run the page.

### Example

1. Drag and drop the **Slide Toggle** component. 
2. Double click the component to display the list of attributes.
3. Input the component field\(s\) with the attribute value\(s\):  

    **`Class`** = _**toggle**_  

    **`Text`** = _**on/off**_

4. Save and run the page.
5. When the page is loaded , the `toggle` class will assign the class name as `toggle`, which can be used to point to a class in a style sheet and the `on/off` is the text that is displayed next to the component.

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
* **Slide Toggle Label:** Display name of the Slide Toggle component..
* **required:** Specify whether the component is required or not.
* **text:** Specify the text to be displayed for the component when the application is run.
* **Label Position:** A drop-down list to select whether the label should appear **`after`** or **`before`** the slide-toggle. Defaults to**`after`**. 
* **name:** Name value to be applied to the **`input`** element \(if present\). The value should either be string or null.
* **id:** A unique id for the Slide Toggle input.
* **\(change\):** The event that will be dispatched each time the Slide Toggle changes its value.
* **Checked:**  A Boolean value to specify whether the Slide Toggle element is checked. Toggle between **`True`** or **`False`**.
* **Color:** A drop-down list which accepts the color based on the angular material theme. You can choose between the following colors, or click the edit button to input the color of your choice:
  * Primary
  * Accent
  * Warn
* **Disabled:** A Boolean value to specify whether the component is disabled or not. Choose `True` or `False`.
* **Disable Drag Value:** A Boolean value to specify if a drag action can trigger value changes in Slide Toggle. Toggle between `True` or `False`.
* **Disable Ripple:** A Boolean value to specify whether ripples are disabled. Toggle between `True` or `False`.
* **Disable Toggle Value:** A Boolean value to specify if a toggle action can trigger value changes in Slide Toggle. Toggle between `True` or `False`.
* **\(dragChange\):**  The event dispatched each time the **Slide Toggle** component is dragged. This event is always emitted when the user drags the slide toggle to make a change greater than 50%
* **\(toggleChange\):** The event dispatched each time the **Slide Toggle** component 

   is toggled. 

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

