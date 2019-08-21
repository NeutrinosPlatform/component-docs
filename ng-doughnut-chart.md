# Doughnut Chart

## Overview

A Doughnut chart is similar to the pie chart but the difference is that doughnut chart has a circular hollow gap in the middle of the chart. This circular hollow gap is called “cutoutPercentage” which represents what percentage of the inner chart should be cut out.

## Usage

A Doughnut Chart is widely used in businesses, mass media, and institutions. Let us consider a health center scenario where a particular hospital wants to plot a chart to record the number of patients admitted to different wards. The chart should represent the overall hospital and be divided into different sections which represent the wards of the hospital. This can be achieved by using the Doughnut Chart where a complete chart represents the hospital and the slices represent the wards of the hospital. There are some other popular use cases as well. Some of them are:

* Pharmaceutical Industries \(indicating the different types of drugs\)
* Industries \(for providing information on different products and services \)
* Government offices \(like revenue department\)
* Retails \(for different types of products they provide\)

### How to use

1. Open the newly created page.
2. Drag and drop the Doughnut Chart from the Ng Charts palette section.
3. Switch to the **Ts** file of the page and then declare the variable and provide values for the following in the component class: 
   * A dataset array \(contains y-axis values and labels of the legend\). For example,

     ```typescript
       public doughnutChartData: Array<any> = [
       {data:[25, 11, 8, 9, 18, 29]}
       ];
     ```

   * A labels array \(contains x-axis values\). For example,

     ```typescript
       public doughnutChartLabels:string[] = ['Emergency & Casualty', 'Labor Ward', 'Endoscopy Ward', 'Coronary Ward', 'Surgical Ward','General Ward'];
     ```

   * Legend value \(either true or false\). For example, 

     ```typescript
       public legend=false;
     ```

   * Options value. For example,

     ```typescript
       public doughnutChartOptions:any = {
       responsive: true
       };
     ```
4. Now switch back to Html file of the page and provide the dataset array name in the \[datasets\] attribute. For example,

   ```text
        [datasets] = doughnutChartData
   ```

5. Provide the labels name in \[labels\] attribute. For example,

   ```text
        [labels] = doughnutChartLabels
   ```

6. Provide the options name in \[options\] attribute. For example, `[options] = doughnutChartOptions`
7. Provide the legend name in \[legend\] attributes. For example, `[legend] = legend`
8. Save the page and run the application.

   \*\*\*\*

**Example**

Consider an example of a hospital that wants to record the percentage of patients admitted to different wards such as emergency & casualty, labor ward, Endoscopy Ward, Coronary Care ward, and Surgical Ward.

| Hospital Wards | Emergency &  Casualty | Labor Ward | Endoscopy Ward | Coronary Ward | Surgical Ward | General Ward |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Patients \(%\)** | 25 | 11 | 8 | 9 | 18 | 29 |

#### Datasets

Here is a sample of a dataset that is declared and initialized in the component class **Ts** file of the project.

```typescript
public doughnutChartData: Array<any> = [
     {data:[25, 11, 8, 9, 18, 29]}
 ];
```

#### Labels

Here is a sample of the labels that are declared and initialized in the component class of **Ts** file of the project.

```typescript
public doughnutChartLabels:string[] = ['Emergency & Casualty', 'Labor Ward', 'Endoscopy Ward', 'Coronary Ward', 'Surgical Ward','General Ward'];
```

#### Legend

Here is a sample of the legend that is declared and initialized in the component class of **Ts** file of the project.

```typescript
  public legend=true;
```

#### Options

Here is a sample of the options that are declared and initialized in the component class of **Ts** file of the project.

```typescript
 public doughnutChartOptions:any = {
   responsive: true };
```

## Associated Attributes

* **Label \(String Array\):** Labels are the identity of the data series in a doughnut chart. It appears in the legend and tooltips. It gives a specific name to each slice in the doughnut chart. For example,

  ```typescript
    public doughnutChartLabels:string[] = ['Emergency & Casualty', 'Labor Ward', 'Endoscopy Ward', 'Coronary Ward', 'Surgical Ward','General Ward'];
  ```

* **Datasets \(JSON Objects Array\):** It is the data of the chart which is framed on a circular slice depending upon the dataset values. For example,

  ```typescript
  public doughnutChartData: Array<any> = [
   {data:[25, 11, 8, 9, 18, 29]}
  ];
  ```

* **chartHover/chartClick \(mouse Events\):** It is an event which appears when the mouse is clicked or placed over the slice of the doughnut chart. For example, displaying label and point value when the mouse is clicked on the slice of the chart or the mouse is moved over it. 
* **Legends \(Boolean\):** It is a name given to the same category of data that is used in plotting the doughnut chart. If it is true, it shows the legends otherwise it does not show.
* **Color \(Color/color hexadecimal code\):** This property provides user desired color to the doughnut chart. For example,

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

