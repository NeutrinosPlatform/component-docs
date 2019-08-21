# Input

## Overview

The Input component is a form control field to input user data such as numbers, alphabets, special characters, password, email, search etc. Input can be used within a form to capture data from the user.

## Usage

The Input component provides an input field where the user can enter data. Input elements are used within a form element to declare input controls that allow users to input data. An input field can vary in many ways, depending on the **`type`** attribute.

### How to use

1. Drag and drop an **`Input`** component. 
2. Double click the component to display the list of attributes that can be used with it.
3. Fill the attributes which are needed and save the page.

### Example

1. Drag and drop an **`Input`** component. 
2. Double click the component to display the list of attributes 

   Input the component field\(s\) with the attribute value\(s\):  

    **`value`**= _**input text here**_  

    **`class`** = ****_**input**_

3. Save and run the page.
4. When the page is loaded, **input text here** is displayed inside the **Input** component. The `input` class is used to point to a class in a style sheet. 

## Associated Attributes

* **Style:** It accepts a string value and affects different properties such as height, width, and color of the component based on the values provided. For example:  `background:orange;height:200px;`.
* **Class:** Used to point to a class in a style sheet. A class contains one or more style statements. Classes are created in the **Styles** editor by clicking  **Styles** in the editor menu. The `class` attribute accepts space separated class names which are defined as shown below:

  ```css
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

* **placeholder:** Used to hold the defined text value. Example **Name** holds the value _**Name**_ for the text field.
* **value:** Used to specify the predefined text that is displayed in the text area. Example _**hello**_ defined in this field will display **hello** in the text field when the application is run.
* **Form Field Appearance:** This field supports 4 different appearance variants:
  * The **`legacy`** appearance is the default style. It shows the input box with an underline underneath it. 
  * The **`standard`** appearance is a slightly updated version of the **`legacy`**appearance that has spacing that is more consistent.
  *  The **`fill`**appearance displays the form field with a filled background box in addition to the underline.
  * The **`outline`**appearance shows the form field with a border all the way around, not just with an underline.

    The **`Prefix`** and **`Suffix`** options are center aligned by default for **`standard`**, **`fill`**, and **`outline`** appearances.
* **required:** Used to specify if the text field should be filled and should not hold empty values. 
* **\[\(Ngmodel\)\]:** Used for two-way data binding. The **`ng-model`**attribute is used to bind the data in your model, to the view presented to the user. The **`ng-model`** attribute is used for binding controls \(such as Input and Text Area components\) in the view into the model.
* **Color:** A drop-down list which accepts the color based on the angular material theme. You can choose between the following colors, or click the edit button to input the color of your choice:
  * Primary
  * Accent
  * Warn
* **name:** Specify a name for the component.
* **type:** Specify the type of text to be input. For example: number, text.
* **\[form control\]:** Used to track values and validations of form elements.
* **readonly:** Specify the display text which cannot be modified by the user.
* **disabled:** A Boolean value that specifies whether the component is disabled or not. Choose `True` or `False`.
* **id:** Specify a unique key for the component.
* **Input Float Label:** The floating label is a text label displayed on top of the form field control when the control does not contain any text. By default, when text is present the floating label floats above the form field control. This field has 3 options. Choose between **`Auto`**, **`Always`** and **`Never`**.
* **Errors:** A button used to enter custom error messages. Refer to [Configure Error messages](https://docs.neutrinos.co/knowledge-center/whats-new/studio-version5#configure-error-messages-in-select-input-and-date-picker-components) for more details.
* **Hints:** These are additional descriptive text messages that appear below the form field's underline. Enter a **`Hint Condition`** and a **`Hint Message`**. An Input component can have up to two hint labels. Therefore, choose **`Start`** or **`End`** as the position of  hint element.  Attempting to add multiple hints to the same side will raise an error. 
* **Label:** Is the label given for the input field. 
* **Suffix Icon:** The icon to be included after the Input tag.
* **\(suffixIconClick\):** The function to be emitted on click of the suffix icon.
* **Prefix Icon:**The icon to be included before the input tag.
* **\(prefixIconClick\)**: The function to be emitted on click of the prefix icon.
* **Prefix:** Custom content that is to be included before the input tag. It will be included within the visual container that wraps the form control
* **Suffix:** Custom content that is to be included after the input tag.

  It will be included within the visual container that wraps the form control

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

