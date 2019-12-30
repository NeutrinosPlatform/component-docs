# N-RICHTEXTEDITOR

n-RichTextEditor provides ready-to-use rich text editors created with a powerful framework. Made with real-time collaborative editing in mind. Its is build using the primary open-source project named [CKEditor](https://ckeditor.com/docs/ckeditor5/latest/index.html). 

# Quick start
- Download n-richtexteditor component from marketplace using the plugin manager. [Rich Text Editor](https://store.neutrinos.co/web/artefact/5dae9cb30bd86577d3d854f1)
- Install the following packages:
```sh
$ npm install --save @ckeditor/ckeditor5-build-classic
```
- After installing the above package, initialize the instance of classic editor to your component (TS)
```sh
export class MyComponent {
    Editor = ClassicEditor;
    // ...
}
```
- Drag and drop a component from the palette list to the required Page inside Neutrinos Platform.
- Assign the ```Editor``` varible to the attribute named ```[editor]``` inside the attribute window.
- Save the page and run the app.
