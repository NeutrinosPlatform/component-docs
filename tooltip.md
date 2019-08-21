# Tooltip

## Overview

The Tooltip component provides a text label that is displayed when the user hovers over or long presses a HTML element. The Tooltip displays information about an element. You can configure the Tooltip to appear above, below, to the left of, or to the right of the HTML element. By default, the position it takes will be below the element. But this can be configured using the `matTooltipPosition`attribute. If the Tooltip is required to switch left/right positions, then the position values before and after should be used instead of left and right respectively.

### How to use

1. Drag and drop the **Tooltip** component to a page container. 
2. Double click the component to display the list of attributes that can be used with it.
3. Fill the required attributes.
4. Save and run the page.

### Example

1. Drag and drop the **Tooltip** component to a page container. 
2. Double click the component to display the list of attributes
3. Input the component field\(s\) with the attribute value\(s\):  

    **`matTooltip`** = _**This is a tooltip**_  

    **`tooltip text`** = _**tooltip**_

4. Save and run the page.
5. When the page is loaded, the text **This is a tooltip** will be displayed when the mouse hovers over the tooltip area and **tooltip** is the text that is displayed on the tooltip field when the page is loaded.

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
* **Tooltip Text:** Specify the text that has to be displayed when the application is run.
* **matTooltip:** Specify the message to be displayed in the Tooltip. The value in this filed has to be a string. 
* **Tooltip Position:** a drop-down list which allows the user to define the position of the Tooltip relative to the parent element. The Drop-down list shows the following options:
  * Below
  * Above
  * Left
  * Right
* **matTooltipShowDelay:** Specifiy the default delay in milli seconds \(ms\) before showing the Tooltip after the `show` method is called.
* **matTooltipHideDelay:**  Specify the default delay in ms before hiding the Tooltip after the `hide` method is called.
* **matTooptipClass:** Specify the classes to be passed to the Tooltip.

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

