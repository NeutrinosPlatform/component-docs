# Select

## Overview

The Select component is used along with one or more option elements. It creates a drop-down list of options for a web form. 

## Usage

A Select component is used to select the list of options available within the select field. When clicked, it displays a drop down list, where the user can select an option.

### How to use

1. Drag and drop the **Select** component. 
2. Double click the component to display the list of attributes that can be used with it.
3. Fill the required attributes 
4. Save and run the page.

### Example

1. Input the component field\(s\) with the attribute value\(s\):

   **`placeholder`** = _**select**_ and **`class`** = _**50.**_

2. Save and run the page.
3. When the page is loaded, `placeholder`  = **select** will display the value **select** and `select` class is the class name that can be used to point to a class in a style sheet.

## Associated Attributes

* **style:** Accepts a string value and affects different properties such as height, width, and color of the component based on the values provided. Example: `background:orange;height:200px;`.
* **class:** Used to point to a class in a style sheet. A class contains one or more style statements. Classes are created in the **Styles** editor by clicking  **Styles** in the editor menu. The `class` attribute accepts space separated class names. They are defined in the "Style" tab as shown below.
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
* **placeHolder:** Used to hold the defined text value. Example “Select” holds the value **Select for the field** when the application is rendered.
* **value:** Specifies the predefined text that is displayed in the select area. When the select field is clicked, it displays the value that is entered in the field. 
* **\[\(ngModel\)\]:** Used for two-way data binding. The **`ngModel`**attribute is used to bind the data in your model to the view presented to the user.
* **required:** Specify if the field is required. 
* **multiple:** A Boolean value that specifies weather the user can select multiple options. Choose **`True`** or **`False`**.
* **\(openChange\)**: Specify the event to be emitted when the select panel has been toggled.
* **\(selectionChange\)**: Specify the event to be emitted when the selected value has been changed by the user.
* **\*ngFor**: Used for iteration.
* **\[value\]**: 
* **optiondata:** Display the options which are entered when the user clicks on the select option.
* **Disabled**: Specify whether the component is disabled or not. Choose **`True`** or **`False`**.
* **\[id\]:** Unique ID of a component which is used for iterating.
* **Errors**: A button used to enter custom error messages. Refer to [Configure Error messages](https://docs.neutrinos.co/knowledge-center/whats-new/studio-version5#configure-error-messages-in-select-input-and-date-picker-components) for more details.

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

