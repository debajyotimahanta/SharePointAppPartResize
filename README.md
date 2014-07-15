#SharePoint App Part resizer plugin
This plugin will resize an app part based on the content in a particualr element. We need to call this when DOM is constrcuted or whenever it changes. It uses SharePoint 2013 resize functionality,which is called by posting the size to the parent.
```javascript
bower install SharePointAppPartResizer
```

### Requirments
+ Needs jquery
+ Needs some kind of AMD (tested with requirejs)

### Overview
Start by includeing this plugin in your app module. Once its included, all you need to do is, initalize the classand as a constrcuter parameter pass in the id of the DOM element which has the content.
```javascript
var resizer = new SharePointResizer("contentRow");
```
