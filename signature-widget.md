# Signature Widget

## Overview

A Signature Widget component is used to create a canvas for handwritten signatures. It contains options to save a signature, undo a stroke, reset the canvas, and cancel the operation.

## Usage

The Signature Widget Component is used when there is a need for handwritten signature. It also removes the need to scan and upload the signature.

### How to use

1. Drag and drop the **Signature Widget** component from palette components **Other** section to the page.
2. Double click on the component and set the attributes value.
3. Save the changes and run the page.

### Example

1. Create a page called **Signature Container**.
2. Drag and drop the **Signature Widget** component.
3. Double click the component.
4. In the **Ts** file, create a property called **`color`** and set its value to _**rgb\(0,0,0\)**_.

   ```typescript
    color = 'rgb(0,0,0)'
   ```

5. Set the value of **`backgroundColor`** to _**color**_.
6. Set the **`dotSize`** attribute to _**3**_ and **`penColor`** to _**rgb\(255,255,255\)**_.
7. Set the value of mode to _**'click-fullscreen'**_ \(with single quotes\). Save the changes.
8. Go to the address where the app is running. Click the pencil icon to display the canvas.
9. The canvas is now black and anything written on it is white.
10. Draw something. Click on save icon \(or the cancel button to exit the canvas\).
11. After the signature is saved, if there is a need to edit it, you can click the pencil icon.

## Associated Attributes

* **Signature Widget Label:** Display name of the File Upload component.
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
* **\[\(imageData\)\]:** This option takes a property name that is defined in **Ts** file which stores the signature image data.
* **\[backgroundColor\]:** Color of the canvas. Color format accepted is **`‘rgb(255,255,255)’`** \(with single quotes\).
* **\[mode\]:** Mode of the canvas. Takes **`‘responsive’`** and **`‘click-fullscreen’`** as its value \(with single quotes\).
* **\[dotSize\]:** Radius of a single dot. Takes number as its value.
* **\[minWidth\]:** Specify the minimum width of a line.
* **\[maxWidth\]:** Specify the maximum width of a line.
* **\[throttle\]:**  Specify the max rate \(per millisecond\) at which the next point is drawn.
* **\[minDistance\]:** Adds the next point only if the previous one is farther than **x** pixels.
* **\[penColor\]:** Specifies the color used to draw the lines. Color format accepted is **`‘rgb(255,255,255)’`** \(with single quotes\).
* **\[velocityFilterWeight\]:** Specify the weight used to modify new velocity based on the previous velocity.
* **\[onBegin\]:** Specify the function that should be executed when stroke begins. It takes the function name as its value. 
* **\[onEnd\]:** Specify the function that should be executed when stroke ends. It takes the function name as its value.

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

