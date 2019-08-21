# Pie Chart

## Overview

A Pie Chart is an excellent chart type for representing the relational proportions between data. It is widely used in the business world as well as in mass media. It represents the data in a pie that is sliced according to the data values.

## Usage

A pie chart is widely used in the business world and mass media. Consider a health center scenario where a particular hospital wants to plot a chart for the record of its patient admitted to different wards. The chart should indicate the overall hospital and should be divided into different sections which represent the wards of the hospital. This can be achieved using a pie chart where a complete pie represents the hospital and slices of the pie chart represent the wards of the hospital. Some of the other popular use cases of a pie chart are:

* Pharmaceutical Industries \(indicating the different types of drugs\)
* Industries \(for providing information on different products and services\)
* Government offices \(like revenue department\)
* Retail \(for different types of products they provide\)

  \*\*\*\*

**How to use**

* Open the newly created page.
* Drag and drop a **Pie Chart** from the **Ng Charts** palette section.
* Switch to the **Ts** file of the page and then declare the variable and provide values for the following in the component class: 
  * A dataset array \(contains y-axis values and labels of the legend\). For example,

    ```typescript
      public pieChartData: Array<any> = [
       {data:[25, 11, 8, 9, 18, 29]}
      ];
    ```

  * A labels array \(contains x-axis values\). For example,

    ```typescript
      public pieChartLabels:string[] = ['Emergency & Casualty', 'Labor Ward', 'Endoscopy Ward', 'Coronary Ward', 'Surgical Ward','General Ward'];
    ```

  * Legend value \(either true or false\). For example, 

    ```typescript
      public legend=false;
    ```

  * Options value. For example,

    ```typescript
      public pieChartOptions:any = {
      responsive: true
      };
    ```
* Now switch back to the Html file of the page and provide the dataset array name in the \[datasets\] attribute. For example,

  ```text
       [datasets] = pieChartData
  ```

* Provide the labels name in \[labels\] attribute. For example,

  ```text
       [labels] = pieChartLabels
  ```

* Provide the options name in \[options\] attribute. For example, `[options] = pieChartOptions`
* Provide the legend name in \[legend\] attribute. For example, `[legend] = legend`
* Save the page and run the application.

### Example

Consider an example of a hospital that wants to plot a chart to record the percentage of patients admitted to different wards such as emergency & casualty, labor ward, Endoscopy Ward, Coronary Care ward, and Surgical Ward.

| Hospital Wards | Emergency &  Casualty | Labor Ward | Endoscopy Ward | Coronary Ward | Surgical Ward | General Ward |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Patients \(%\)** | 25 | 11 | 8 | 9 | 18 | 29 |

#### Datasets

Here is a sample of a dataset that is declared and initialized in the component class **Ts** file of the project.

```typescript
public pieChartData: Array<any> = [
     {data:[25, 11, 8, 9, 18, 29]}
 ];
```

#### Labels

Here is a sample of the labels that are declared and initialized in the component class of **Ts** file of the project.

```typescript
public pieChartLabels:string[] = ['Emergency & Casualty', 'Labor Ward', 'Endoscopy Ward', 'Coronary Ward', 'Surgical Ward','General Ward'];
```

#### Legend

Here is a sample of the legend that is declared and initialized in the component class of **Ts** file of the project.

```typescript
  public legend=true;
```

#### Options

Here is a sample of the options that are declared and initialized in the component class of **Ts** file of the project.

```typescript
 public pieChartOptions:any = {
   responsive: true };
```

## Associated Attributes

* **Label \(String Array\):** Labels are the identity of the data series in a chart. It appears in the legend and tooltips. It gives a specific name to each slice in the pie chart. For example,

  ```typescript
    ChartLabels:Array<any> = ['January', ‘February’, 'March', 'April', 'May', 'June', 'July'];
  ```

* **Datasets \(JSON Objects Array\):** It is a data of the chart which is framed on a circular slice whose length depends on the dataset values. For example,

  ```typescript
  pieChartData: Array<any> = [{data: [69, 72, 82, 79, 92], label: 'Net Profit Margin (%)'} ];
  ```

* **chartHover/chartClick \(mouse Events\):** It is an event which appears when the mouse is clicked or placed over the pie chart. For example, displaying label and point value when the mouse is clicked on the chart or mouse is moved over the chart. 
* **Legends \(Boolean\):** It is a name given to the same category of data that is used in plotting the pie chart. If it is true, it shows the legends otherwise it does not show.
* **Color \(Color/color hexadecimal code\):** This property provides user desired color to the pie chart. For example, 

  ```css
    background-color: #92a8d1;
  ```

* **Key:** Key is used to provide user custom key point into the chart. It is like a user’s custom parameter provided to the chart section.
* **Value:** It is a value of the key that the user provided manually.
* **Style:** It accepts a string value and affects the different properties \(height, width, color etc.\) of the component based on the values provided \(eg. background:orange;height:200px;\).
* **Class:** "Class" attribute is used to point to a class in a style sheet. A class contains one or more style statements. Classes are created inside the "Style" tab which is opened by selecting the "Style" side menu. The "Class" attribute accepts space separated class names \(eg. class1 class2\) which are defined in the "Style" tab as shown below.

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

  **Support**

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

