# Sidenav Container

## Overview

The Sidenav Container is the container for Sidenav components. “Sidenav” component has meaning only when it is placed inside the “Sidenav Container” component. Everything that is not contained within the “Sidenav“ component and contained within "Sidenav Container" component will appear as main content that is outside the sidenav bar.

## Usage

Sidenav container is used whenever a sidenav is required. Sidenav cannot exist outside sidenav container component.

### How to use

1. Drag and drop a **Sidenav Container** component from the **Navigation** section.
2. Drag and drop a **Sidenav** component inside the **Sidenav Container** component.
3. Populate the **Sidenav** component with the content that is required in the side navigation of that page.
4. Save the changes and run the page.

### Example

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

* **Sidenav Container Label:** Specify the display name of the Sidenav Container.
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
* **Auto Size:** Specify whether to automatically resize the container whenever the size of any of its drawers changes.

{% hint style="warning" %}
Enabling this option can cause layout thrashing by measuring the drawers on every change detection cycle. Can be configured globally via the`MAT_DRAWER_DEFAULT_AUTOSIZE` token.
{% endhint %}

* **Has Back Drop:** Specify whether the drawer container should have a backdrop while one of the sidenavs is open. If explicitly set to `true`, the backdrop will be enabled for drawers in the `side` mode as well.
* **\(backdropClick\):** Specify the event emitted when the drawer backdrop is clicked.

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

