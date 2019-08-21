---
description: >-
  Grid Tile allows you to create a container of list of particular rows and
  columns. It can be used alone as well as inside the grid-list.
---

# Grid Tile

## Description

A Grid Tile component is used to display a list of items.The column inside the Grid Tile component will contain the attribute and the row will contain the data of a particular attribute. 

The data to be displayed can be iterated by providing **`ngFor`** loop which can access data from the array and display on the screen.

## Usage

1. Drag and drop a **Grid Tile** component.
2. Set the attributes of the component.
3. Depending to the properties that you set, the list item will be displayed on the screen.

### Example

**Display a Grid List component with 3 items. Also add a Grid Tile component within the Grid List.** 

1. Drag and drop a **Grid List** component to a page container.
2. Set the following values in the Attributes window:
   1. **`cols`**= _**4**_ to display 4 columns.
   2. **`rowHeight`** = _**100px**_
3. Drag and drop a **Grid Tile** component inside the **Grid List** and set the following values for the **Grid Tile** component:
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

4.  So in the above example, the grid has two columns, and tile is an array which has four items containing string values \(labels\). The labels will be displayed using the`ngFor` loop.

5. Save and Run the page.

6. A table with four items will be displayed inside the **Grid List**.

## Associated Attributes

* **`Grid Tile Label`:** Used to give a label to the Grid Tile.
* **`style`:** Accepts a string value that affects different properties of Grid Tile such as height, width, and color, based on the values provided. For example: `background:orange:height:200px`.
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

* **`ngFor`:** A loop used to iterate through array objects and get the data. The syntax of ``**`ngFor`** is **`*ngFor="let d of data"`** where **`d`** _****_is a loop variable and **`data`** is an array or object from which the data will be accessed. 
* **`rowspan`:** Defines the number of rows a cell should span. In a normal row the **`rowspan`** is always set to 1. This attribute is required when there is a requirement to change the row size. For example, when a row size  is to be two times the size of the normal row, in such a case, the **`rowspan`** value will be set to 2.
* **`colspan`:** Defines the number of columns a table cell should span. In a normal column, the `colspan` is always set to 1. This attribute is required only when there is a requirement to change the column size. For example, when a column size  is to be two times the size of the normal column, in such a case, the **`colspan`** value will be set to 2.

  \*\*\*\*

**Support**

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 + 

