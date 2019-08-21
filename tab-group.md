# Tab Group

## Overview

The Tab Group component is a container component that is used to contain one or more Tab components. Tab components should always be contained in the Tab Group component.

## Usage

A Tab Group component is used whenever tab\(s\) are used. A Tab component can not exist outside of the Tab Group component.

### How to use

1. Drag and drop the **Tab Group** component from the palette components **Navigation** section.
2. Drag and drop **Tab** components inside the **Tab Group** component.
3. Set the **`label`** attribute of the **Tab** components.
4. Drag and drop the components needed within each **Tab** component.
5. Save the changes and run the page.

### Example

1. Create a page.
2. Drag and drop the **Tab Group** component from the palette components **Navigation** section.
3. Drag and drop  three **Tab** components inside the **Tab Group** component.
4. Set the value of the **`label`** property the tabs to _**Tab1**_, _**Tab2**_, and _Tab3_ respectively. 
5. Drag and drop a Card component \(from palette components **Navigation** section\) within each tab.
6. Set height of each card to **`100px`**. That is, update the **`style`** attribute to _**height:100px;**_.
7. Set the color of each card. Example - Update the **`style`** attribute

   to _**color:pink;**_

8. Save the changes and run the page.
9. When the page is rendered, you will see three tabs. You can navigate between each tabs by clicking on it.

## Associated Attributes

* **Tab Group Label:** Display name of the Tab Group.
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
* **animationDuration:** Specify the duration for the Tab animation. This attribute will be normalized to milliseconds if no units are set.
* **backgroundColor:** Specify the background color of the Tab Group.
* **Color:** A drop-down list which accepts the color based on the angular material theme. You can choose between the following colors, or click the edit button to input the color of your choice:
  * None
  * Primary
  * Accent
  * Warn
* **Dynamic Height:** A Boolean value to specify whether the tab group should grow to the size of the active tab.  Choose between `True` or `False`.
* **headerPosition:** Specify the position of the Tab header.
* **selectedIndex:** Specify the index of the selected tab.
* **\(animationDone\):** Specify the event emitted when the body animation has completed.
* **\(focusChange\):** Specify the event emitted when focus has changed within a tab group.
* **\(selectedIndexChange\):** Specify the output to enable support for two-way binding on **`selectedIndex.`**

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

