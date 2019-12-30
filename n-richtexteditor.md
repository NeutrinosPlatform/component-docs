# N-RICHTEXTEDITOR

n-RichTextEditor provides ready-to-use rich text editors created with a powerful framework. Made with real-time collaborative editing in mind. Its is build using the primary open-source project named [CKEditor](https://ckeditor.com/docs/ckeditor5/latest/index.html). 

# Quick start
- Downoload n-richtexteditor component from marketplace using the plugin manager.
- Drag and drop a component from the palette list to you page
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
- Assign the ```Editor``` varible to your component attribute named ```[editor]``` 
- Save the page and run your application
