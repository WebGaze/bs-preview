# bs-preview

## How to use this tool
To use the Bootstrap Preview tool, simply include the following elements in your template: 

```html
<html>
  <head>
    <!-- #bs-theme required for the script to inject the css urls -->
    <link id="bs-theme" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet">
  </head>
  <body>
    <nav class="navbar navbar-default" role="navigation">
      <!-- Navbar content... -->
    </nav>
    <div class="container" role="main">
      <!-- #bs-previer required for the script to inject the menu -->
      <div id="bs-previewer"></div>
      <!-- Body content... -->
    </div>
    <!-- Make sure to include the bootstrap.js files if needed -->
    <script src="https://code.jquery.com/jquery-3.2.1.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
    <script src="js/bs-previewer.js"></script>
  </body>
</html>
```

The wrapper div can be placed anywhere in your template and will conform to your responsiveness or lack there of. You will be presented with 3 options in the menu that is generated:

* **Theme**  
 A list of themes to apply to your page. Simply click on any of the theme names to apply them to your page.  
 By default this list includes the Default and Styled versions of [Bootstrap](http://getbootstrap.com/) as well as the full offering of [Bootswatch](http://bootswatch.com/) themes.  
 <small>_All themes are property of their respective owners._</small>
* **Current Theme: Bootstrap Default**  
 This button displays your currently applied theme. When clicked, it will cycle through the full list of themes, one by one.
* **Navbar View: Default**  
 This button displays your currently applied navbar class. When clicked, it will cycle between ```.navbar-default``` and ```.navbar-inverse```

The index.html file included is built from the Bootstrap 3 example template. However, by including the elements above into any template you will get the same functionality. Everything is generated on the page, so you can use this with any template library you would like. I use this with [PUG](https://pugjs.org), but I've tested it with plain HTML 5 and Handlebars as well.
