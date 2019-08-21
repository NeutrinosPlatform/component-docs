# Toolbar

## Overview

A Toolbar is a container for headers, titles, menus or actions that perform specific functions.

## Usage

Toolbars are designed to provide easy and immediate access to users' most frequently used functions or provide relevant information about the page or application.

### How to use

1. Drag and drop the **Toolbar** component from the palette component **Navigation** section into a page’s container where the toolbar component should be rendered .
2. Fill in the **`Content`** attribute with the value the toolbar should contain.

### Example

1. Create a page.
2. Drag and drop the **Toolbar** component from the palette component **Navigation** section.
3. Set the **`Content`** attribute to _**I'm a toolbar**_.
4. Save and run the page.

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
* **Color:** A drop-down list which accepts the color based on the angular material theme. You can choose between the following colors, or click the edit button to input the color of your choice:
  * Primary
  * Accent
  * Warn
* **content:** Specify the content to be displayed inside the toolbar. Its value can be plain text or valid html tags. Example: 
  * Plain text: **This is a toolbar**.
  * HTML tags:

    ```markup
      <button mat-button>I'm a button</button>
    ```

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

