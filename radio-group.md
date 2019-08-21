# Radio Group

## Overview

A Radio Group is a group of radio buttons. It allows a user to select at most one radio button from a set. Checking one radio button that belongs to a radio group unchecks the previously checked radio button within the same group.

## Usage

A Radio Group component is used to contain radio buttons.

### How to use

1. Drag and drop the **Radio Group** component into a page container
2. Drag and drop one or more **Radio Buttons** inside the **Radio Group**. 
3. Double click each of the radio buttons and set their attributes
4. Double click the **Radio Group** component and set the required attributes.
5. Save  and run the page.

### Example

1. Drag and drop the **Radio Group** component into a page container.
2. Drag and drop two **Radio Buttons** inside the **Radio Group**. Click a radio button and set the following properties in the Attributes window:

    **`Checked`** = **oncheck\(\)**  

    **`Value`** = **option1**  

3. Click the other radio button and set the following ****properties in the Attributes window:**`Checked`** = **oncheck\(\)**  and **`Value`** = **option2**  
4. Open the TS window by clicking![](../../../.gitbook/assets/image%20%281%29.png) in the editor window. Insert the following function:

   ```typescript
    onclick() { 
        alert("radio buttn clicked");
    }
   ```

5. Click the Radio Group component and set the following ****properties in the Attributes window: 

 **`Labelposition`** = _**after**_   and **`Name`** = _**rdgroup**_

6. Save and run the page.

7.When the page is run, you will see two radio buttons namely **option1** and **option 2** in a radio group named **rdgroup**.

## Associated Attributes

* **radio Group label:** Display name of the Radio Group.
* **style:** Accepts a string value and affects different properties such as height, width, and color of the component based on the values provided. Example: `background:orange;height:200px;`.
* **class:** Used to point to a class in a style sheet. A class contains one or more style statements. Classes are created in the **Styles** editor by clicking  **Styles** in the editor menu. The **`class`** attribute accepts space separated class names. They are defined in the **`Style`** tab as shown below.
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
* **\[value\]:** Used to specify a value for the radio group. Should equal the value of the selected radio button if there is a corresponding radio button with a matching value. If there is no such corresponding radio button, this value persists, to be applied in case a new radio button is added with a matching value.
* **\[\(ngModel\)\]:** Used for two-way data binding. The **`ng-model`** attribute is used to bind the data in your model to the view presented to the user.
* **name:** An attribute used to group radio buttons for a unique selection. All radio buttons inside this group will use this name.
* **selected:** The currently selected radio button. If set to a new radio button, the radio group value will be updated to match the newly selected button.
* **\(change\):** Specify the event to be emitted when the checked state of a radio button changes. Change events are only emitted when the value changes due to user interaction with the radio button.
* **Label Position:** Defines the label to appear after or before the radio button. Defaults to **`after`**.
* **required:** On page rendering, this field is used to check whether the user has to select a radio button in this radio group.
* **label:** Is the label given to the Radio Group.

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

