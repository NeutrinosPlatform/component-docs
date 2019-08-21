# Menu Item

## Overview

A Menu item is a list of options from which an option can be selected to perform a specific operation. A Menu Item is the individual option that can be selected within a Menu component. A Menu Item is always contained in the Menu component.

## Usage

Menu Items are what makes up a Menu. Menu Items are used to provide options within a Menu.

### How to use

1. Drag and drop the **Menu** component from the palette components **Navigation** section.
2. Set the **`matMenu`** attribute to a string value.
3. Drag and drop the **Menu Item** component\(s\) inside the **Menu** component.
4. Set the **`MenuItemName`** of Menu Item component to a string value.
5. Drag and drop the **Menu Button** component to the desired position and set **`MenuName`**  attribute.
6. Set the **`matMenuTriggerFor`** attribute to the same value as the `matMenu` attribute of the Menu component.
7. Save the changes and run the page.

### Example

1. Create a page.
2. Drag and drop the **Menu** component.
3. Set the **`matMenu`** attribute to _**menu**_.
4. Drag and drop three **Menu Item** components inside the **Menu** component.
5. Set the **`MenuItemName`** attributes of **Menu Item** components to _**item1, item 2, and item 3**_  respectively.
6. Drag and drop the **Menu Button** component to the desired position and set **`MenuName`** attribute to _**Menu**_ and **`matMenuTriggerFor`** attribute to _**menu**_.
7. Save the changes and run the page.
8. When the page is rendered, clicking the **Menu** button will reveal the list of menu items  as **item1**, **item2**, and **item3**.

## Associated Attributes

* **Menu Item Label:** Display name of the Menu Item.
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
* **MenuItemName:** Specify the name of the menu item that appears in the application. Takes string as its value. 
* **Disabled:** A Boolean value to specify whether the Menu Item is disabled. Choose between `True` or `False`.

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

