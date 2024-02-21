To develop the website in this repository, I use simple HTML commands and some CSS styling to enhance its applicability. Initially, I established the general structure using HTML. The general structure looking like:
```
<!DOCTYPE html>
<html lang="en">
<html>
  <head>

  </head>
  <body>

  </body>
  <footer>

  </footer>
</html>
```
Firstly, we need to import some 'libraries' to access certain characters and icons. Additionally, you must link CSS files to the main HTML file to enable HTML to recognize the style changes on the webpage.
```
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<link rel="stylesheet" href="style.css"> 
<script src="https://kit.fontawesome.com/982561656d.js"></script>
<title>Shamkhalil's Partfolio</title>
```
After we have done so, we can move onto the header of the page, in the html sense the code is quite simple:
```
<div class="header">
  <div class="header-text">
    <p>Khalilov Shamkhalil</p>
  </div>
</div>
```
The CSS portion is straightforward. The primary elements of the CSS code include setting the background color and adjusting margins to eliminate any white spacing issues.
```
.header {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background-color: #15155b;
    color: #fff;
    padding: 5px 4px;
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 1;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.header-text {
    font-family: 'Courier New', Courier, monospace;
    font-size: 20px;
    font-weight: 500;
    display: flex;
    align-items: center;
    margin-left: 25px;
}

.header button {
    background-color: #553E11;
    color: #fff;
    border: none;
    padding: 10px 20px;
    margin: 0 10px;
    cursor: pointer;
}

.header button:hover {
    background-color: #777;
}
```
