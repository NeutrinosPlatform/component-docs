# Sidenav

## Overview

The Sidenav component allows you to add side content to a full screen app. Sidenav typically contains links to different pages or sections in the app. Sidenav is a fixed layout whose slide-in and slide-out activity can be bound to an action \(For example- Button press, checkbox etc.\). The Sidenav component has meaning only when it is placed inside the Sidenav Container component.

## Usage

Sidenav is useful when the user needs to have immediate access to the most used pages/components of an app.

### How to use

1. Drag the **Sidenav** component from the **Navigation** section and drop it inside the **Sidenav Container** component.
2. Populate the **Sidenav** component with the content that is required in the side navigation of that page.
3. Save the changes and run the page.

### Example \(not correct - needs to be updated\)

1. Create a page called **home**.
2. Drag and drop the **Sidenav Container** into the page.
3. Drag and drop the **Sidenav** component inside the **Sidenav Container**.
4. Drag and drop a **HTML5** component into the page.
5. Write an anchor tag inside that HTML component with `href` attribute set to _**http://www.neutrinos.co**_  and `target` attribute to _**blank**_.

   ```markup
    <a href="http://www.neutrinos.co">neutrinos</a>
   ```

6. Save the changes and run the page.
7. When the page loads, clicking the button will open the Neutrinos website.

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
* **Sidenav Mode:** A drop-down list to choose the side navigation mode. Sidenav can render in one of three different ways based on the `mode` property.
  * **`over`** - Sidenav floats over the primary content, which is covered by a backdrop
  * **`push`** - Sidenav pushes the primary content out of its way, also covering it with a backdrop
  * **`side`** - Sidenav appears side-by-side with the main content, shrinking the main content's width to make space for the sidenav.
* **Opened:**  A Boolean value used to decides whether the Sidenav should be opened. Choose between `True` or `False`.
* **Sidenav Position:** A drop-down list to choose the side navigation position. Position can either be **`start`** or **`end`** which places the side content on the left or right side. Default is **`start`**.
* **fxLayout:** Specify the flex direction and whether the contents should be wrapped or not. Example: **`fxLayout=column wrap`**
* **\(opened\):** Takes function name as the value. This function is defined in the **Ts** file and is executed when the Sidenav is opened.
* **\(closed\):** Takes function name as the value. This function is defined in the **Ts** file and is executed when the Sidenav is closed.
* **\(toggle\):** Takes function name as the value. This function is defined in the **Ts** file and is executed when the Sidenav is toggled.
* **Auto Focus:** A Boolean value to specify whether the drawer should focus the first focusable element \(automatically\) when opened. Choose between `True` or `False`.
* **Disable Close:** A Boolean value to specify whether the drawer can be closed with the escape key or by clicking on the backdrop. Choose between `True` or `False`.
* **\(onPositionChanged\):** Event emitted when the drawer's position changes.
* **\(openedChange\):** Event emitted when the drawer open state is changed.
* **fixedBottomGap:**  Specify the gap between the bottom of the Sidenav and the bottom of the view port when the Sidenav is in fixed mode. This option accepts only numeric value.
* **Fixed InView Port:** A Boolean value to specify whether the sidenav is fixed in the viewport. Choose between **`True`** or **`False`**.
* **fixedTopGap:** Specify the gap between the top of the Sidenav and the top of the viewport when the sidenav is in fixed mode. This option accepts only numeric value.

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

