# Date Picker

## Overview

The Date Picker component is used to present an interface for users to select the date. Tapping on the component will display a picker interface that can be used to select a date.

## Usage

Date Picker component is used to select a date from the calendar. It omits the need for the user to enter the date manually.

### How to use

1. Drag and drop the **Date Picker** component. 
2. Double click the component to display the list of attributes that can be used with it.
3. Fill the required attributes.
4. Save and run the page.

### Example

1. Drag and drop the **Date Picker** component. 
2. Double click the component to display the list of attributes 
3. Input the component field\(s\) with the attribute value\(s\):  

    **`opened`**= _**opened\(\)**_  

    **`placeholder`** = _**datepicker**_  

4. Open the TS window by clicking![](../../../.gitbook/assets/image%20%281%29.png) in the editor window. Insert the following function:

   ```typescript
    opened() { 
        alert("Datepicker opened");
    }
   ```

5. Save and run the page.
6. After the page is loaded, **opened\(\)** is the event that will be emitted when the Date Picker component is opened and **datepicker** is the text that will be displayed in the datepicker field when the page is loaded. 

## Associated Attributes

* **style:** Accepts a string value and affects different properties such as height, width, and color of the component based on the values provided. Example: `background:orange;height:200px;`.
* **class:** Used to point to a class in a style sheet. A class contains one or more style statements. Classes are created in the **Styles** editor by clicking  **Styles** in the editor menu. The `class` attribute accepts space separated class names. They are defined in the **`Style`** tab as shown below:
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
* **value:** Specify the new value for the target Date Picker input. Value has to be either null or the letter “D”.
* **min:** Specify the minimum valid date. The value should be either null or the letter “D” 
* **max:** Specify the maximum valid date. The value should be either null or the letter “D”
* **\[startAt\]:** Specify the initial date to open the calendar. It should be in the format: `D | null`.
* **Start View:** Specify the view that the calendar should start in. It should be in the format: `'month' | 'year'`.
* **touchUi:** Specify whether the calendar UI is in touch mode. In touch mode, the calendar opens in a dialog rather than a pop-up window, and elements have more padding to allow for bigger touch targets.
* **id:** Specify the id for the datepicker calendar. The value should be a string.
* **\(dateChange\):** Is an event that is emitted when the selected date is changed.
* \(dateInput\):
* **Opened:** Specify whether the calendar should be open or not. Choose between `True` or `False`.
* **Disabled:** Specify whether the datepicker pop-up should be disabled or not. Choose between `True` or `False`.
* **\(open\):** Is an event called when the calendar is open.
* **\(close\):** Is an event called when the calendar is closed.
* **matDatepickerFilter:** Specify the function that can be used to filter out dates within the datepicker. The value should be given in this format. `(date: D | null)` `=> boolean(true or false)`
* **\[\(ngModel\)\]:** Used for two-way data binding. The `ng-model` attribute is used to bind the data in your model to the view presented to the user.
* **name:** Specify the name for the date picker.
* **picker:** Specify the ID for the date picker component.
* **Errors:** A button used to enter custom error messages. Refer to [Configure Error messages](https://docs.neutrinos.co/knowledge-center/whats-new/studio-version5#configure-error-messages-in-select-input-and-date-picker-components) for more details.

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

