# NDirectives

## Camera

* Description :

    Custom directive for upload file from mobile only based on cordova. 

    If you want to use this add **n-camera** custom directive any component.

* Input
  * \[cameraOptions\] = "{entityName: 'profile', metadata: {key: 'example@neutrinos.co'}}"
  * entityName - collection Name - string
    * example

        entityName = 'profile'
  * metadata - object
    * example

        metadata = {key: 'example@neutrinos.co'}
* Output
  * \(onsuccess\) - success method
    * example

        \(onsuccess\) = success\($event\)
  * \(onerror\) - error method
    * example

        \(onerror\) = error\($event\)

## File Download

* Description :

    Custom directive for download file. 

    If you want to use this add **n-download** custom directive any component.

* Input
  * \[downloadOptions\] = "{entityName: 'profile', metadata?: {key: 'example@neutrinos.co'}, fileId?: '5a659b8d8fa0d80af3551f70'}"
  * In \[downloadOptions\] either fileId nor metadata is required. If both exist it will take only metadata.
  * entityName - collection Name - string
    * example

        entityName = 'profile'
  * metadata - object
    * example

        metadata = {key: 'example@neutrinos.co'}
  * fileId - individual file Id - string
    * example

        fileId = '5a659b8d8fa0d80af3551f70'
* Output
  * \(onsuccess\) - success method
    * example

        \(onsuccess\) = success\($event\)
  * \(onerror\) - error method
    * example

        \(onerror\) = error\($event\)

## File Upload

* Description :

    Custom component for upload file from browser. 

    If you want to use this add **File Upload** component.

* Input
  * \[uploadOptions\] = "{entityName: 'profile', metadata: {key: 'example@neutrinos.co'}}"
  * entityName - collection Name - string
    * example

        entityName = 'profile'
  * metadata - object
    * example

        metadata = {key: 'example@neutrinos.co'}
* Output
  * \(onsuccess\) - success method
    * example

        \(onsuccess\) = success\($event\)
  * \(onerror\) - error method
    * example

        \(onerror\) = error\($event\)

## Cam Scanner

* Description :

    Custom directive for document scanner from cordova devices.

    If you want to use this add **n-scan** custom directive any component.

* Input
  * \[scanOptions\] = "{entityName: 'profile', metadata: {key: 'example@neutrinos.co'}, sourceType: 0, doUpload : true}"
  * entityName - collection Name - string
    * example

        entityName = 'profile'
  * metadata - object
    * example

        metadata = {key: 'example@neutrinos.co'}
  * sourceType - whether camera or gallery - number
    * example

        sourceType = 0
  * doUpload - whether to upload directly or return imageUri instead - boolean
    * example

        doUpload = true
* Output
  * \(onsuccess\) - success method
    * example

        \(onsuccess\) = success\($event\)
  * \(onerror\) - error method
    * example

        \(onerror\) = error\($event\)

## Barcode Reader

* Description :

    Custom directive for barcode / QR code scanning from cordova devices.

    If you want to use this add **n-barcode** custom directive to any component.

* Input \(Optional will take defaults if input isn't provided\)
  * \[barcodeOptions\]

    ```text
    [barcodeOptions] = "{
          preferFrontCamera: boolean,
          showFlipCameraButton: boolean,
          showTorchButton: boolean,
          torchOn: boolean,
          saveHistory: boolean,
          prompt: "Place a barcode inside the scan area",
          resultDisplayDuration: 1500,
          formats: "DATA_MATRIX,UPC_A,UPC_E,EAN_8,EAN_13,CODE_39,CODE_93,CODE_128,CODABAR,ITF,RSS14,MSI,AZTEC",
          orientation: string,
          disableAnimations: boolean,
          disableSuccessBeep: boolean

      }"
    ```
* Output
  * \(onsuccess\) - success method
    * example

        \(onsuccess\) = success\($event\)   


        The object \(for example result\) returned on success contains the following values.    


        result.text that contains the text obtained from the barcode.   


        result.format which is the format of the code returned.   


        result.cancelled is a boolean value which is true if user cancelled the operation and false if user didn't cancel. This value is always false in the success callback function.
  * \(onerror\) - error method
    * example

        \(onerror\) = error\($event\)

## Video

* Description : Custom directive for for capturing video from cordova devices. If you want to use this add **n-video** custom directive to any component.
* Input
  * \[videoOptions\] = "{entityName: 'profile', metadata: {key: 'example@neutrinos.co'}}"
* Output
  * \(onsuccess\) - success method
    * example

        \(onsuccess\) = success\($event\)
  * \(onerror\) - error method
    * example

        \(onerror\) = error\($event\)

## Text to Speech

* Description : Custom directive for converting text to speech in cordova devices. If you want to use this add **n-tts** custom directive to any component.
* Input
  * \[ttsOptions\] = "{text: 'Enter your text', locale: 'en-GB', rate: 1}"
  * text - String to be converted to speech - string
    * example

        text = 'Say Hi'
  * locale - language of speech - string
    * example

        locale = 'en-GB'
  * rate - speed of speech, value from 0 to 1 - number
    * example

        rate = 0.75
* Output
  * \(onsuccess\) - success method
    * example

        \(onsuccess\) = success\($event\)
  * \(onerror\) - error method
    * example

        \(onerror\) = error\($event\)

## Shake

* Description : Custom directive for detecting shakes in cordova devices. If you want to use this add **n-shake** custom directive to any component.
* Input
  * \[shakeOptions\] = "{sensitivity:30, start:true}"
  * sensitivity - sensitivity for shake detection - number
    * example

        sensitivity = 30
  * start - true to start shake detection, false to stop shake detection - boolean
    * example

        start = true
* Output
  * \(onsuccess\) - success method
    * example

        \(onsuccess\) = success\($event\)
  * \(onerror\) - error method
    * example

        \(onerror\) = error\($event\)

## Optical Character Recognition

* Description : Custom directive for Optical Character Recognition in cordova devices. If you want to use this add **n-ocr** custom directive to any component.
* Input
  * \[ocrOptions\] = "{quality:100, correctOrientation: true, uriOrBase:0, returnType:1}"
  * quality - quality of the image taken - number
    * example

        quality = 100
  * correctOrientation - correct the orientation of the image taken - boolean
    * example

        correctOrientation = true
  * uriOrBase - The type of image \(can take values 0, 1, 2, 3, 4\) - number
    * example

        uriOrBase = 0
  * returnType - The return text format of OCR \(can take values 0, 1, 2, 3\) - number
    * example

        returnType = 1
* Output
  * \(onsuccess\) - success method
    * example

        \(onsuccess\) = success\($event\)
  * \(onerror\) - error method
    * example

        \(onerror\) = error\($event\)

## Fingerprint

* Description : Custom directive for fingerprint Recognition of saved fingerprints in cordova devices. If you want to use this add **n-fingerprint** custom directive to any component.
* Input
  * \[fingerprintOptions\] = {clientId: 'string', clientSecret: 'string'}
  * clientId - Unique clientId for your app \(any string as per users' choice\) - string
    * example

        clientId = 'Neutrinos'
  * clientSecret - Unique clientSecret for your app \(any string as per users' choice\) - string
    * example

        clientSecret = 'Password'
* Output
  * \(onsuccess\) - success method
    * example

        \(onsuccess\) = success\($event\)
  * \(onerror\) - error method
    * example

        \(onerror\) = error\($event\)

