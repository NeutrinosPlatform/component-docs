# image-carousel

## Overview

Carousel is used to show images in a slideshow. This template is responsive so it will display gorgeously on all screen types including mobiles and computers. In addition, our carousel will automatically change its size to fit the image’s size.

## Usage

Carousels are often used to display a series of looping images. There are some other popular usages of carousel. Some of them are:

* Teasers   
  * Articles     
  * Entire sections of web pages

### How to Use

1. Download the carousel template from Neutrinos store.  
2. Install the template into N-Studio. 
3. When creating a new app, select the carousel template from the **ENTER APP DETAILS** menu and click on the create button.
4. Create a component \(Example:carousel\) 
5. In **TS** file 
6. Import services: one service based on user requirements \(Example: imageservice\) and another, carousel service, which contains **observable media**- used for tracking the responsiveness.

   ```typescript
   import{imageserviceService}from'../../services/imageservice/imageservice.service';
   ```

   ```typescript
   import { carouselserviceService } from  '../../services/carouselservice/carouselservice.service';
   ```

* Inject the two services in 'constructor'

  ```typescript
  constructor(private  imgService:imageserviceService,private  cService:carouselserviceService) {
  }
  ```

* Inside **class**, declare the variables used

  ```typescript
    imagedata : String ;
    limit : any ;
  ```

* In **ngOnInit**

  `this.imageData = this.imgService.getImages();`

> **imagedata** - Variable used in imageservice. **imgservice** - Keyword for the service.

* write a function

  ```typescript
    ngDoCheck() { 
    this.limit = this.cService.assignLimit(1, 2, 4); 
    }
  ```

> **limit** - Variable used in carouselservice. **cservice** - Keyword for the service. **ngDoCheck\(\)** - Function used for tracking the responsiveness.

* In **HTML** file

  Drag and drop a custom html to call the child component

  ```markup
  <bh-carousel [imageData]="imageData"[limitImage]="limit" *ngIf="imageData"></bh-carousel>
  ```

> **carousel**- Name of the child component.

## Support

* **Devices:** Android, iOS  
* **Browsers:** Latest version of all modern browsers  
* **Dependencies version**  :
  * Angular CLI version: 6.0.0 +  
  * Cordova version: 7.1.0 +

