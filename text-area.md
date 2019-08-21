# Text Area

## Overview

Text Area component is a form control field to input user data such as numbers, alphabets, special characters, password, email, search etc. Input can be used within the forms to capture the data from the user.

## Usage

Text Area component specifies an input field where the user can enter data. Input elements are used inside a form element to declare input controls that allow users to input data. An input field can vary in many ways, depending on the `type` attribute.

### How to use

1. Drag and drop the **Text Area** component to the page container. 
2. Double click the component to display the list of attributes that can be used with it.
3. Fill the attributes which are needed and save the page.

### Example

1. Drag and drop the **Text Area** component to the page container. 
2. Double click the component to display the list of attributes
3. Input the component fields with the following attribute values:  

    **`value`** = _**Input text here**_  

    **`class`** = _**textarea**_

4. Save and run the page.
5. When the page, a **Text Area** component with text **Input text here** will be displayed. You can use the **textarea\(\)** class to point to a class in a style sheet. 

## Associated Attributes

* **style:** Accepts a string value and affects different properties such as height, width, and color of the component based on the values provided. Example: `background:orange;height:200px;`.
* **class:** Used to point to a class in a style sheet. A class contains one or more style statements. Classes are created in the **Styles** editor by clicking  **Styles** in the editor menu. The `class` attribute accepts space separated class names. They are defined in the `Style` tab as shown below:
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
* **placeholder:** Used to hold the defined text value. 
* **value:** Specify the predefined text that is to be displayed in the text area when the application is run. For example, if you define _**hello**_ this field, **hello** will be displayed in the text field when the application is run.
* **required:** Specify if the text field should be filled and should not hold empty values. The value should be Boolean, that is, either `true` or `false`.
* **\[\(ngModel\)\]:** Used for two-way data binding. The `ng-model` attribute is used to bind the data in your model to the view presented to the user. The `ng-model` attribute is used for binding controls such as input and text area in the view, into the model.
* **Color:** A drop-down list which accepts the color based on the angular material theme. You can choose between the following colors, or click the edit button to input the color of your choice:
  * Primary
  * Accent
  * Warn
* **name:** Specify the name for the text field.
* **\[readonly\]: Specify the** display text which cannot be modified by the user.
* **Disabled:** Specify whether the component should be disabled or not. Choose `True` or `False`.

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

