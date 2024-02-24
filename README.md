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
And so the header will look, like this:
![header](https://github.com/SHamkhalil/Web-Programming-Front-end-/blob/main/header.png?raw=true)
Here, there are two redundancies, specifically the header button and the header button:hover. Initially, there were buttons at the top of the page; however, afterwards, it seemed as if they were redundant due to the website's length.
![buttons displayed](https://github.com/SHamkhalil/Web-Programming-Front-end-/blob/main/buttons.png?raw=true)
Then came time to write the about me section, the same section was rehashed and used in the projets section. The only difference being the the flex-direction was changed from row to row-reversed.
A general structure of these sections was looking like:
```
<div class="about">
            <img src="placeholder.jpg" alt="Partfolio-img">
            <div class="about-text">
                <p style="font-size: 25px; font-family:Georgia, 'Times New Roman', Times, serif;">About me</p>
                <hr>
                <p>I'm Shamkhalil Khalilov, a student at the Technical University of Azerbaijan. I've been studying there for 2 years and have a wide variety of interests ranging from competitive programming to graphical engineering and even music. Over the past 6 months, I have competed in a dozen or so competitions on websites like Codeforces and AtCoder. In addition to the aformentioned, I have also participated in the 2023 ICPC semi-finals. Furthermore, I have developed a "brute-force" ray tracing application in C++.</p>
                <p>Regarding my skills, I have gained considerable proficiency in both C++ and Python. Primarily, I use C++ for most of my projects, but when it comes to analyzing raw data or similar tasks, I prefer to use Python due to its simple syntax.</p>
                <p>I'm planning to relocate to the Enschede, Netherlands this August to pursue my academics at Twente University, where I plan to study Computer Science and Mathematical Analysis. My future goal is to use the knowledge I have to specialize in graphical engineering as a profession. </p>
                <hr>
            </div>
        </div>
```
I didn't have a picture of myself at hand, so I just used a placeholder that I had at hand.
Structurally, these sections were the same in the way that a general container to hold every item was created, and then there are some sub-containers to hold text or images.
Styling through CSS was quite simple so there is no point in dissecting it. The general structure of it looked something like:
```
.about {
    margin-top: 75px;
    padding: 20px;
    display: flex;
    align-items: center;
}

.about img {
    max-width: 275px;
    margin-right: 20px;
}

.about p {
    font-family: Arial, Helvetica, sans-serif;
    color: #333;
    font-size: 16px;
    line-height: 1.5;
}

.about-text {
    flex: 1;
}

.about-text p {
    color: #333;
    font-size: 16px;
    line-height: 1.5;
    margin: 0 0 10px;
}
```
The last part of the website was the footer, which is essentially a rehashing of the header. The footer is also a rectangle at the end of the page; however, while the header has a relative position, meaning that it moves wherever the scroll commands it to, the footer is static, meaning it has a fixed position. Additionally, there are some icons on the footer, which were made possible using the Font Awesome library of icons.
```
    <footer class="footer">
      <div class="footer-content">
        <p style="font-family: Georgia, 'Times New Roman', Times, serif;"><i class="fa-solid fa-envelope"></i> xalilovwamik@gmail.com</p>
        <ul class="footer-links">
          <li><a href="https://www.linkedin.com/in/shamkhalil-khalilov-178380245/"><i class="fa fa-linkedin" aria-hidden="true"></i></a></li>
          <li><a href="https://github.com/SHamkhalil"><i class="fa-brands fa-github"></i></a></li>
          <li><a href="https://docs.google.com/document/d/1qHNt9cxH15KM-hLxxr4GVTQgO7wvub2k5nsXLWXMDAE/edit?usp=drive_link"><i class="fa-solid fa-file-pdf"></i></a></li>
          <li><a href="https://codeforces.com/profile/Shamkhalil"><i class="fa fa-code"></i></a></li>
        </ul>
      </div>
    </footer>
```
Each of the icons is clickable and leads to the pages that I own. Additionally, an email is provided; however, the email can only be copied by selecting it.
Again the CSS behind the footer is quite literally the same as in the header, so there is no point in dissecting it.
At the end the footer would look like something like this:
![footer](https://github.com/SHamkhalil/Web-Programming-Front-end-/blob/main/footer.png?raw=true)
At the very end if the provided code is run the following website should appear:
![website_overview](https://github.com/SHamkhalil/Web-Programming-Front-end-/blob/main/overview.png?raw=true)
