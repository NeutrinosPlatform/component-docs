# Table

## Overview

The Table component provides a styled data table that can be used to display rows of data. The Table component focused on a single responsibility to efficiently render rows of data in a performant and accessible way.

The simplest way to provide data to the table is by passing a data array to the table's `dataSource` input. The table will take the array and render a row for each object in the data array. The data source is meant to serve a place to encapsulate any sorting, filtering, pagination, and data retrieval logic specific to the application.

A data source is simply a base class that has two functions: **`connect`** and **`disconnect`**. The **`connect`** function will be called by the table to receive a stream that emits the data array that should be rendered. The table will call **`disconnect`** when the table is destroyed.

### How to use

1. Drag and drop a **Table** component to the page container. 
2. Optionally add columns, drop columns, paginator, and filter components.
3. Double click the Table component to display the list of attributes that can be used with it.
4. Double click the column, drop column, paginator, and filter components added within the table, and set its attributes.
5. Fill the attributes
6. Save and run the page.

### Example

* Drag and drop a **Table** component into the page container.
* Initialize the data in the **`TS`** file by adding the following data to the table's **`TS`** script:

```bash
// Data table configuration (Sample Data)
   PeriodicElement = [
       { position: 1, name: 'Hydrogen', weight: 1.0079, symbol: 'H' },
       { position: 2, name: 'Helium', weight: 4.0026, symbol: 'He' },
       { position: 3, name: 'Lithium', weight: 6.941, symbol: 'Li' },
       { position: 4, name: 'Beryllium', weight: 9.0122, symbol: 'Be' },
       { position: 5, name: 'Boron', weight: 10.811, symbol: 'B' },
       { position: 6, name: 'Carbon', weight: 12.0107, symbol: 'C' },
       { position: 7, name: 'Nitrogen', weight: 14.0067, symbol: 'N' },
       { position: 8, name: 'Oxygen', weight: 15.9994, symbol: 'O' },
       { position: 9, name: 'Fluorine', weight: 18.9984, symbol: 'F' },
       { position: 10, name: 'Neon', weight: 20.1797, symbol: 'Ne' },
   ];
```

* Create 4 columns to accommodate the data from the data source.
* Open the component's attribute window. In the **`[datasource]`** field, give the name of the datasource as _**PeriodicElement**_.
* Open the attribute window of each column and input _**{{table.position}}**_ in the **`mapping`** field.
* Save and run the page.

## Associated Attributes

#### **Basic Properties: These properties remain the same for all Table components.**

* **`style`:** Accepts a string value that affects different properties of the Card such as height, width, and color, based on the values provided. For example: `background:orange:height:200px`.
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

### Other Properties: These properties are unique to each component.

### Table:

* **Table label:** Specify the display name of the table.
* **\[dataSource\]:** Specify the table's source of data.
* **Show Header:** Allows you to choose if you want to show the Table's header or not. Choose `True` of `False`.

#### Column:

* **Header Label:** Specify the display name of the column.
* **Mapping:** Specify the data to be displayed in the column. For example: **`{{table.position}}`**
* **Sort:** Allows you to sort column data. Choose between **`True`** of **`False`**.

#### Droppable Column:

* **Sort Key:** Key to sort/arrange the data. For example- ascending.
* **Sort:** Allows you to sort column data. Choose between `True` of `False`.
* **columnid:** Unique ID for the component.
* **Header Label:** Specify the display name of the Droppable Column.

#### Pagintor: 

* **\[length\]:**  Specify the length of the total number of items that are being paginated.
* **\[page Size\]:** Specify the number of items to display on a page.
* **\[pageSizeOptions\]:** Specify the set of provided page size options to display to the user. The page size options include 5, 10, 25, and 100.
* **\(page\):** The event emitted when the paginator changes the page size.

#### Filter:

* **\(tableFilterFunction\):** The function used to perform the table filter.
* **placeholder:** Specify the name of the filter to be displayed on the screen.
* **Layout Direction:** The position to display the filter.
* **fxFlex:** Size of the filter component.

#### Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +



