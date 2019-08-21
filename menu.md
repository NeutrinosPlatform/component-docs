# Menu

## Overview

A Menu is a set of options presented to the user of a computer application to help the user find information or execute a function.

## Usage

Menu is used when the user is to be provided with the ability to select from a list of options without consuming the GUI layout.

### How to use

1. Drag and drop the **Menu** component from the palette component **Navigation** section.
2. Set the **`matMenu`** attribute to a string value.
3. Drag and drop the **Menu Item** component\(s\) inside the **Menu** component.
4. Set the **`MenuItemName`** of  the **Menu Item** component to a string value.
5. Drag and drop the **Menu Button** component to the desired position and set **`MenuName`** attribute.
6. Set the **`matMenuTriggerFor`** attribute to the same value as the _**matMenu**_ of the **Menu** component.
7. Save the changes and run the page.

### Example

1. Create a page called **Neutrinos Home Page**.
2. Drag and drop the **Menu** component.
3. Set the **`matMenu`** attribute to _**menu**_.
4. Drag and drop  three **Menu Item** components inside the **Menu** component.
5. Set the **`MenuItemName`** attribute of menu items to _**item1**_, _**item2**_, and _**item3**_.
6. Drag and drop the **Menu Button** component to the desired position and set **`MenuName`** attribute to _**Menu**_ and **`matMenuTriggerFor`** attribute to _**menu**_.
7. Save the changes and run the page.
8. When the page is rendered, clicking the **Menu** button will reveal the list of menu items  as **item1**, **item2**, and **item3**.

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
* **xPosition:** Specify the horizontal position of the menu list. Values can be **`before`** or **`after`**.
* **yPosition:** Specify the vertical position of the menu list. Values can be **`above`** or **`below`**.
* **templateRef:** Creates a template reference variable. Takes string as its value.
* **items:** List of items inside of a menu.
* **matMenu:** Specify the parent menu of the current menu panel. This field accepts String values. This value should be same as **`matMenuTriggerFor`** attribute’s value of the **Menu** component.
* **Has Back Drop:** Specify whether the menu has a backdrop. Choose between **`True`** or **`False`**.
* **Overlap Trigger:** Specify whether the menu should overlap the menu trigger. ****Choose between **`True`** or **`False`**.
* **\(closed\):** The event emitted when the menu is closed.
* **direction:** Specify the layout direction of the menu.
* **parentMenu:** Specify the parent menu of the current menu panel.

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

