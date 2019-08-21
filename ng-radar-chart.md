# Radar Chart

## Overview

A Radar Chart is also known as a web chart, cobweb chart or spider chart. It plots the data as an irregular polygon. All the axes in this chart are connected from a common center point on which data values are plotted. This plotting method forms a spider web-like structure which gives a proper comparison between the data groups.

## Usage

A Radar Chart is widely used in hospitals, in the cricket world, in industries etc. Let us consider a scenario from a particular industry where a human resource \(HR\) team wants to prepare a chart on the performance of the candidates under different skill specifications during the selection process. In this case, the HR should be able to take a glance at all the candidates' performance scores. This can be achieved using a radar chart. It can be used to plot all the candidates' performance scores in a spider web form and provide an excellent understandability from it. There are some other popular use cases where a radar chart is used. Some of them are:

* Government offices
* Retail
* Hospitals
* Experimental surveys

### How to use

1. Open the newly created page.
2. Drag and drop a **Radar Chart** from the **Ng Charts** palette section.
3. Switch to the **Ts** file of the page and then declare the variable and provide values for the following in the component class: 
   * A dataset array \(contains y-axis values and labels of the legend\). For example,

     ```typescript
       public radarChartData:Array<any> = [
       {data: [7, 8, 6, 9, 7, 9], label: 'Dayashankar'},
       {data: [6, 7, 7, 8, 6, 8], label: 'Oliver'}
       ];
     ```

   * A labels array \(contains x-axis values\). For example,

     ```typescript
       public radarChartLabels:string[] = ['Communication Skills', 'Technical Knowledge', 'Team Work', 'Meeting Deadline', 'Problem Solving', 'Punctuality'];
     ```

   * Legend value \(either true or false\). For example, 

     ```typescript
       public legend=false;
     ```

   * Options value. For example,

     ```typescript
       public radarChartOptions:any = {
       responsive: true
       };
     ```
4. Now switch back to the Html file of the page and provide the dataset array name in the \[datasets\] attribute. For example,

   ```text
        [datasets] = radarChartData
   ```

5. Provide the labels name in \[labels\] attribute. For example,

   ```text
        [labels] = radarChartLabels
   ```

6. Provide the options name in \[options\] attribute. For example, `[options] = radarChartOptions`
7. Provide the legend name in \[legend\] attribute. For example, `[legend] = legend`
8. Save the page and run the application.

### Example

Consider an example of an industry where the HR \(Human Resource\) team hires some professionals. They conduct different activities to monitor the following skills of the candidates; communication skills, technical knowledge, teamwork, meeting deadline, problem-solving, and punctuality. The head HR should be able to glance at the candidates' performance through a graph or chart which reflects a good comparison between all candidates. This can be achieved using a radar chart. For example,

| Candidates | Communication Skills | Technical Knowledge | Team Work | Meeting Deadline | Problem Solving | Punctuality |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Dayashankar** | 7 | 8 | 6 | 9 | 7 | 9 |
| **Oliver** | 6 | 7 | 7 | 8 | 6 | 8 |

#### Datasets

Here is a sample of a dataset that is declared and initialized in the component class **Ts** file of the project.

```typescript
public radarChartData:Array<any> = [
    {data: [7, 8, 6, 9, 7, 9], label: 'Dayashankar'},
    {data: [6, 7, 7, 8, 6, 8], label: 'Oliver'}
  ];
```

#### Labels

Here is a sample of the labels that are declared and initialized in the component class of **Ts** file of the project.

```typescript
public radarChartLabels:string[] = ['Communication Skills', 'Technical Knowledge', 'Team Work', 'Meeting Deadline', 'Problem Solving', 'Punctuality'];
```

#### Legend

Here is a sample of the legend that is declared and initialized in the component class of **Ts** file of the project.

```typescript
  public legend=true;
```

#### Options

Here is a sample of the options that are declared and initialized in the component class of **Ts** file of the project.

```typescript
 public radarChartOptions:any = {
   responsive: true };
```

## Associated Attributes

* **Label \(String Array\):** Labels are the identity of the data series in a chart. It appears in the legend and tooltips. It gives a specific name to each section of the chart. For example,

  ```typescript
    public radarChartLabels:string[] = ['Communication Skills', 'Technical Knowledge', 'Team Work', 'Meeting Deadline', 'Problem Solving', 'Punctuality'];
  ```

* **Datasets \(JSON Objects Array\):** It is the data of the chart, framed on the spider web format that is proportional to the data values. For example,

  ```typescript
  public radarChartData:Array<any> = [
  {data: [7, 8, 6, 9, 7, 9], label: 'Dayashankar'},
  {data: [6, 7, 7, 8, 6, 8], label: 'Oliver'}
    ];
  ```

* **chartHover/chartClick \(mouse Events\):** It is an event which appears when the mouse is clicked or placed over the chart area. For example, displaying label and point value when the mouse is clicked on the section of the chart or mouse is moved over it. 
* **Legends \(Boolean\):** It is a name given to the same category of data that is used in plotting the radar chart. If it is true, it shows the legends otherwise it does not show.
* **Color \(Color/color hexadecimal code\):** This property provides user desired color to the radar chart. For example, 

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

