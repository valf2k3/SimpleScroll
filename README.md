# [SimpleScroll](https://valf2k3.github.io/SimpleScroll)
 This code will help you show items on scroll

# Install
Download the scroll Api.js and scrollSpy.css files and include them:
```
<link type="text/css" rel="stylesheet" href="scrollApi.css"/>
<script type="text/javascript" src="scrollApi.js"></script>
```

# How to use?
Example:
```
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>Simple API for show items on scroll</title>
        <link type="text/css" rel="stylesheet" href="scrollApi.css"/>
        <link type="text/css" rel="stylesheet" href="css/main.css"/>
    </head>
    <body>
        <script type="text/javascript" src="scrollApi.js"></script>
        <div class="container">
            <div class="item red">
                <b>Simple Scroll<p>For small projects</p></b>
            </div>
            <div class="item green">
                <b>Simple for use<p>Does not require special knowledge</p></b>
            </div>
            <div class="item blue">
                <a href="https://github.com/valf2k3/SimpleScroll">Download</a>
            </div>
        </div>
        <script type="text/javascript">
            let sa = new scrollApi({'time': 1500});
            let items = document.getElementsByClassName("item");
            for(let i = 0; i < items.length; i++){
                sa.addElement(items[i]);
            }
            sa.init();
        </script>
    </body>
    </html>
```
