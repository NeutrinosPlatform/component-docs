# Menu Button

## Overview

A Menu Button is always associated with a Menu component that contains a list of Menu Items. When a Menu button is clicked, the associated Menu Items will be shown.

## Usage

A Menu button is used to provide an interface for the user to trigger a Menu List. Menu appears where the menu button exists.

### How to use

1. After creating a **Menu**, drag and drop the **Menu Button** component to the desired position and enter a value for the **`MenuName`** attribute.
2. Set the **`matMenuTriggerFor`** attribute to the same value as the **`matMenu`** attribute of the Menu component.
3. Save the changes and run the page.

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
* **MenuName:** Specify the name of the menu button to appear in the application. It accepts String values.
* **Color:** A drop-down list which accepts the color based on the angular material theme. You can choose between the following colors, or click the edit button to input the color of your choice:
  * Primary
  * Accent
  * Warn
* **\[matMenuTriggerFor\]:** Used to reference the menu instance that the trigger is associated with. This value should have the same value as the **`matMenu`**attribute of the associated **Menu** component. This field accepts String values.

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

