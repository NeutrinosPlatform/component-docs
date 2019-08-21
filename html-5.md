---
description: The HTML5 component provides you with an HTML editor to compose web content.
---

# HTML5

### Description

The HTML5 component is used to design components to be displayed in web format. When you drag and drop a HTML5 component, the page container by default displays a HTML editor inside the HTML 5 component. This editor can be used to compose web content.. 

### Usage

1. Drag and drop a **HTML5** component to the page container. A `HTML Editor` is already added into the component by default.
2. Click the **HTML Editor** to open an editor in the page container.
3. Design the HTML document according to your app requirement by adding tags. A few of the commonly used tags are described below:
   1. **`Div:`**Used to add a division or a section in an HTML document.
   2. **`Span:`**Used to group inline-elements in a HTML document.
   3. **`Paragraph:`**Used to insert a paragraph in a HTML document.
   4. **`Header1 - 6:`** Used to insert a header tag in a HTML document.
   5. **`Label:`**Used to put a display text on the component describing what purpose it has for the user.
   6. **`Caption:`** Used to add a caption to an HTML table.
   7. **`Fieldset:`** Used to group related elements in a form. This tag draws a box around the related elements.
   8. **`iFrame:`** An inline frame is used to embed another document within the current HTML document.
4. Optionally add another **`HTML Editor`** if required.
5. Save and run the page.

### Example

1. Drag and drop a  **HTML5**  component to a page container.
2. Click the **`HTML Editor`** inside the component.
3. In the editor below, enter the following HTML tags:

```text
<title>Neutrinos</title>
<h1>Rapid app development platform</h1>
<p>A new-age app development platform which empowers business and IT teams to build enterprise apps.</p>
```

When the app gets deployed, you will see a HTML page titled Neutrinos with a heading and a paragraph.

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
* Element type: A drop-down list containing the following HTML5 elements:
  * **`Div:`**Used to add a division or a section in an HTML document.
  * **`Span:`**Used to group inline-elements in a HTML document.
  * **`Paragraph:`**Used to insert a paragraph in a HTML document.
  * **`Header1 - 6:`** Used to insert a header tag in a HTML document.
  * **`Label:`**Used to put a display text on the component describing what purpose it has for the user.
  * **`Caption:`** Used to add a caption to an HTML table.
  * **`Fieldset:`** Used to group related elements in a form. This tag draws a box around the related elements.
  * **`iFrame:`** An inline frame is used to embed another document within the current HTML document.

**Support**

* **Devices:** Android, iOS
* **Browsers:** Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 + 

