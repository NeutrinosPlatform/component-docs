---
description: >-
  A Grid List contains a list of particular rows and columns. The column will
  contain the attribute and the row will contain the data of the particular
  attribute.
---

# Grid List

### Description

A Grid List component offers a user defined grid-based layout system, with rows and columns, making it easier to layout and align content.

Use the **`cols`** attribute to set the number of columns in the grid. The number of rows will be automatically determined based on the number of columns and the number of items. 

## Usage

1. Drag and drop a **Grid List** component to the page container. 
2. Set the component attributes and configure how it should be displayed. 
3. Depending to the properties set, the list item will be displayed on the screen.

### Example

**Display a Grid List component with 3 items. Also add a Grid Tile component within the Grid List.** 

1. Drag and drop a **Grid List** component to a page container.
2. Set the following values in the Attributes window:
   1. **`cols`**= _**4**_. So that four columns are displayed.
   2. **`rowHeight`** = _**100px**_
3. Drag and drop a **Grid Tile** component inside a **Grid List** and set the following values for the grid Tile component:
   1. **`colspan`** = _**1**_
   2. **`rowspan`** = _**1**_
   3. **`Label` =** Refer the code below
   4. **`ngFor` =** Refer the code below

```markup
Displaylist.html file
<mat-grid-list cols="2" rowHeight="100px">
  <mat-grid-tile
      *ngFor="let tile of tiles" // in *ngFor attribute
         {{tile.text}}    // label attribute
  </mat-grid-tile>
</mat-grid-list>
```

```typescript
Displaylist.ts
       tiles: Tile[] = [
       {text: 'One'},
       {text: 'Two'},
       {text: 'Three'},
    {text: 'Four'},
  ];
```

5. So in the above example grid has two columns, and tile is a array which has four items which contains string value that are basically labels. So using `ngFor` the labels will be displayed.

6. Save and Run the page

7. A table with four items will be displayed inside a **Grid List**.

## Associated Attributes

* **`Grid List Label`:** Used to give a label to the Grid List describing what purpose it has for the user.
* **`style`:** Accepts a string value that affects different properties of Grid List such as height, width, and color, based on the values provided. For example: `background:orange:height:200px`.
* **`class`:** Used to point to a class in a style sheet.  Each class contains one or more style statements defined in the **Style** editor. The `Class` field accepts space separated class names such as `class1 class2` , where each class is defined in the Style editor as shown below:

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

* **`Cols`:** Used to specify the number of columns in the list. This is a mandatory field and accepts an integer value. After you provide the column value, the structure of the list will be created.
* **`gutterSize`:** Gutters provide spacing between the content that is to be displayed. The gutter size can be set to any `px`, `em`, or `rem` value. If no units are specified, `px` units are assumed. By default the gutter size is **`1px`**.
* **`rowHeight`:** The height of the rows in a grid list. Row height for the list can be calculated in three ways:

  * **`Fixed height`:** Provide a fixed height. The height can be in `px`, `em`, or `rem` units. If no units are specified, `px` units are assumed. 
  * **`Ratio`:** This ratio is measured in `column-width:row-height`, and must be passed in with a colon in between. For example: _**4:3**._
  * **`Fit`:** If you set the **`rowHeight`** property to **Fit,** this mode automatically divides the available height by the number of rows. For the property to do so, you must first set the height of the Grid List or its container.

    \*\*\*\*

  **Support**

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 + 

