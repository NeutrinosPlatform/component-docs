# Polar Area Chart

## Overview

A Polar Area Chart provides detailed comparison information. The radius of the sector differs according to the value in datasets whereas in pie chart the radius of each slice is same. In this chart, the difference in data can be found easily by looking at the radius of the slice.

## Usage

A Polar Area Chart is used as an alternative to the pie chart in different fields such as hospitals, retails, industries, data science and analytics etc. Let us consider a health centre scenario where a particular hospital wants to plot a chart to record the patients admitted to different wards. The chart should indicate the overall hospital and should be divided into different sections which represent the wards of the hospital. This can be done by using a pie chart however it would not provide proper readability. Therefore, in this case, if the polar area chart is used, it would provide global understanding just from the structure of the chart. There are some other popular use cases. Some of them are:

* Industries
* Government offices
* Hospitals
* Government surveys
* Experimental surveys

### How to use

1. Open the newly created page.
2. Drag and drop a **Polar Area Chart** from **Ng Charts** palette section.
3. Switch to the **Ts** file of the page and then declare the variable and provide values for the following in the component class: 
   * A dataset array \(contains y-axis values and labels of the legend\). For example,

     ```typescript
       public polarChartData: Array<any> = [
       {data:[25, 11, 8, 9, 18, 29]}
       ];
     ```

   * A labels array \(contains x-axis values\). For example,

     ```typescript
       public polarChartLabels:string[] = ['Emergency & Casualty', 'Labor Ward', 'Endoscopy Ward', 'Coronary Ward', 'Surgical Ward','General Ward'];
     ```

   * Legend value \(either true or false\). For example, 

     ```typescript
       public legend=false;
     ```

   * Options value. For example,

     ```typescript
       public polarChartOptions:any = {
       responsive: true
       };
     ```
4. Now switch back to the Html file of the page. 
5. Then provide the dataset array name in the \[datasets\] attribute. For example,

   ```text
        [datasets] = polarChartData
   ```

6. Provide the labels name in \[labels\] attribute. For example,

   ```text
        [labels] = polarChartLabels
   ```

7. Provide the options name in \[options\] attribute. For example, `[options] = polarChartOptions`
8. Provide the legend name in \[legend\] attribute. For example, `[legend] = legend`
9. Save the page and run the application.

   **Example**

   Consider an example where a hospital wants to plot a chart to record the patients admitted to the different wards of the hospital such as emergency & casualty, labor ward, Endoscopy Ward, Coronary Care ward, and Surgical Ward.

| Hospital Wards | Emergency &  Casualty | Labor Ward | Endoscopy Ward | Coronary Ward | Surgical Ward | General Ward |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Patients \(%\)** | 25 | 11 | 8 | 9 | 18 | 29 |

#### Datasets

Here is a sample of a dataset that is declared and initialized in the component class **Ts** file of the project.

```typescript
public polarChartData: Array<any> = [
        {data:[25, 11, 8, 9, 18, 29]}
];
```

#### Labels

Here is a sample of the labels that are declared and initialized in the component class of **Ts** file of the project.

```typescript
public polarChartLabels:string[] = ['Emergency & Casualty', 'Labor Ward', 'Endoscopy Ward', 'Coronary Ward', 'Surgical Ward','General Ward'];
```

#### Legend

Here is a sample of the legend that is declared and initialized in the component class of **Ts** file of the project.

```typescript
  public legend=true;
```

#### Options

Here is a sample of the options that are declared and initialized in the component class of **Ts** file of the project.

```typescript
 public polarChartOptions:any = {
   responsive: true };
```

## Associated Attributes

* **Label \(String Array\):** Labels are the identity of the data series in a chart. It appears in the legend and tooltips. It gives a specific name to each section of the chart area. For example,

  ```typescript
    public polarChartLabels:string[] = ['Emergency & Casualty', 'Labor Ward', 'Endoscopy Ward', 'Coronary Ward', 'Surgical Ward','General Ward'];
  ```

* **Datasets \(JSON Objects Array\):** It is data of the chart, framed on different sectors. For example,

  ```typescript
  public polarChartData: Array<any> = [
   {data:[25, 11, 8, 9, 18, 29]}
  ];
  ```

* **chartHover/chartClick \(mouse Events\):** It is an event which appears when the mouse is clicked or placed over the sector of the polar area chart. For example, displaying label and point value when the mouse is clicked on the sector of the chart or mouse is moved over it. 
* **Legends \(Boolean\):** It is a name given to the same category of data that is used in plotting the polar area chart. If it is true, it shows the legends otherwise it does not show.
* **Color \(Color/color hexadecimal code\):** This property provides user desired color to the polar chart. For example, 

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

