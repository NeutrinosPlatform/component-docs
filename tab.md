# Tab

## Overview

Tabs are used to navigate between different views within the same context. Only one view is rendered at a time. Tabs should always be used inside a Tab Group component.

## Usage

Tabs are useful for containing and navigating between contextually related, but distinct contents.

### How to use

1. Drag and drop the **Tab Group** component from the palette component **Navigation** category.
2. Drag and drop the **Tab** component\(s\) inside the **Tab Group** component.
3. Set the **`label`** attribute of the **Tab** component\(s\).
4. Drag and drop the components needed within each **Tab** component.
5. Save the changes and run the page.

### Example

1. Create a page.
2. Drag and drop the **Tab Group** component from the **Navigation** category.
3. Drag and drop two **Tab** components inside the **Tab Group** component.
4. Set the values of the Tab's**`label`**” property to _**Image**_ and _**Tab2**_ respectively.
5. Drag and drop **Image** component from the Form Controls section and set its attributes.
6. Drag and drop two **Card** components from the Layout section into each of the tabs.
7. Set height of each card, that is, set **`style`** = **`height:50px;`**.
8. Set the color of each card.
9. Save the changes and run the page.
10. When the page renders, you can navigate between tabs.

## Associated Attributes

* **Tab Label:** Display name of the tab.
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
* **label:** Specify the name of the tab as seen in the app. It accepts String value.
* **Disabled:** A Boolean value to specify whether the Tab is disabled. Choose between `True` or `False`.
* **isActive:** A Boolean value to specify whether the Tab is currently active. Choose between **`True`** or **`False`**.
* **position:** Specify the relatively indexed position where 0 represents the center, negative is left, and positive represents the right.
* **index:** Specify the index of the currently selected tab.
* **origin:** Specify the initial relatively index origin of the tab. It provides context of what position the tab should originate from.

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

