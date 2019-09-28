
# CSEduHackUMBC19
Resources for HackUMBC Intro to Web Development  
Presented by Computer Science Education Club  
Developed by Zoee Leckron

__We're doing everything fast, here are the notes!__
- This repository will have all of our resources (https://github.com/zleckron/cseduHackUMBC19.git)

__Setup and Downloads__
1. Download Sublime3: [sublime.com/3](https://www.sublimetext.com/3)
2. Download Git: [git-scm.com](https://git-scm.com/downloads)
  (we will not be talking about SSH keys in this workshop)
3. Download Sublime Merge (for Git): [sublimemerge.com](https://www.sublimemerge.com/)
4. Create a GitHub account: [github.com](https://github.com/)
5. In the web version of GitHub, create a New repository
  *__IMPORTANT:__* Name your new repository to `username.github.io`, where `username` is your username on GitHub.
  (Otherwise hosting on Github will not work)
6. In the web version of GitHub, copy the HTTPS path to your repository
7. Open Sublime Merge and paste the copied HTTPS path into the Source URL field
  If you don't see the Source URL field, go to File > Clone Repository.  
  You can change the destination path just make sure you remember it.

__In Sublime__
- Make a file and save it as `index.html` (the "index" part of the name is not very significant but the html file extension is) __in your username.github.io__ folder
- With your saved .html file open, type `<ht` then hit tab to add standard HTML tags automatically
- Try adding some words in between the `<title></title>` tags! Whatever you put between these tags will show up in the tab when you open the file (see __Testing__)

__Testing__
- Find the `index.html` file in your file explorer and double click it. It should open in your default browser
- You should see your changes in the tab

__Debugging__  
Are you not seeing something you want to see on your webpage? Or seeing something that you don't want to see?
- In Chrome, right click > Inspect to pull up the developer console
- In Firefox, go to Tools > Web Developer > Inspector
You can make small changes to your code in the inspector and see them rendered. This does not change the code in your html file(s).  
This will open up the HTML source code, Styles (CSS, which we haven't talked about yet), and the Console for JavaScript (which we also haven't talked about yet)

__Uploading to Git__
- Open Sublime Merge. If it is not already open to the repository you cloned earlier, use File > Open Repository
- You should see that there is 1 untracked file and that it is `index.html`
- Double click the Stage All button
- You will see the option to Commit 1 File. You are required to add a commit message before committing. This message should help tell you (and anyone else) what change was made.
- If you want to, confirm that the commit message and file changes are showing up in the web version of your repository (on Github.com)

__Workflow__
1. Make a change to your file(s) and save
2. Open `index.html` in the browser and check it out (double click on the file as you did before)
    If you already have the file open in the browser, you can just refresh the page to see your changes
3. Confirm that you want to keep these changes
4. In Sublime Merge, follow the above directions in __Uploading to Git__
5. The changes will be reflected in your website at `https://username.github.io`
6. Loop back to step 1
It is up to you how often you commit and push your changes. You do not have to push every time you commit, but your changes will only show up once you push.

_HTML Fast Facts!_
1. Pretty much everything in HTML is in _tags_ enclosed in an opening and closing tag with angle brackets!
    - Normal HTML tag to make a paragraph: `<p>literal string content</p>`
    - Tag to make a line break (doesn't ): `<br>`
  You can assume that most tags require a closing tag like `</p>` but there are exceptions like `<br>` to look out for
2. Strings don't need to go in quotes! See above paragraph example - the words "literal string content" will appear on the HTML page.  

Headers in HTML
```
<!-- header sizes range from the largest <h1></h1> to smallest <h6></h1>
<h1>Big header</h1>
```  
Tables in HTML
```
<table>
	<tr>
		<th>header for first column</th>
		<th>header for second column</th>
		... <!-- repeat for each column in your table -->
	</tr>
	<tr>
		<td>data for first column, first row</td> <!-- td = table data -->
		<td>data for second column, first row</td>
		... <!-- repeat for each column in your table -->
	</tr>
  .
  .
  .
  <!-- repeat <tr></tr> for each row in your table -->
</table>
```  
Buttons in HTML  
(you can put an image in an HTML button too but I won't be covering that right now)  
```
<!-- buttons with text -->
<button>LABEL</button>
<button><a href="pastelinkhere" target="_blank">LABEL</a></button>
```  
Navigation Bars in HTML  
(here we are linking to different sections in one file; you can also link to different HTML pages by specifying their path)
```
<nav>
  <!-- The section name should match the id attribute that you want to jump to -->
  <a href="#mysectionname">LABEL</a>
  .
  .
  .
  <section id="schedule">...</section>
</nav>
```

_Making it look good: Cascading Style Sheets_
- File > New or `Cmd-n` to make a new file, save it to `styles.css` (CSS style sheet) in the same folder as `index.html`  
- Link your stylesheet to your HTML header section:  
  `<link rel="stylesheet" type="text/css href="styles.css">`  

CSS rule syntax:
  ```
    myselector {
      property:value;
    }
  ```  
See the `styles.css` file in the PredevelopedSources for many examples  

CSS Resources  
- Color picker: [htmlcolorcodes.com](https://htmlcolorcodes.com/color-picker/)
- Photos that are safe to use: [Unsplash.com] (https://unsplash.com/)

_Making it do things (animations, etc)_
1. File > New or `Cmd-n` to make a new file, save it to `script.js` (JavaScript)
Javascript function syntax:
  ```javascript
  function function_name(argument) {
    // body...
  }
  ```  
2. Link the JavaScript file in your HTML header: `<script src="script.js"></script>`

__Programming Practices__  
Accessibility:
We want to encourage good programming practices. To make your website appealing to a variety of users, you should follow some compliance guidelines.
1. Article with an easy-to-understand list of ADA compliance website issues (I recommend you skip to the issues): https://www.digitalauthority.me/resources/ada-compliance-website/
2. Check for at least 4.5:1 ratio of color contrast: https://webaim.org/resources/contrastchecker/
3. Having good alternative text for images and descriptive link text is important!
    - Alt text in HTML image tags looks like this: `<img src="truegrit.jpg" alt="Chesapeake Bay Retriever True Grit, best mascot in Maryland">`
    - Descriptive link text looks like this: `<a href="https://www.hackumbc.org/">HackUMBC Home Page 2019</a>`  

__Copyrights & Legal Stuff__  
Credit photos! Even though photos from Unsplash are free, it's courteous to credit the photographer

__Tips for Speed__  
HTML shortcuts in Sublime
1. Auto Tags: With your saved .html file open, type `<ht` then hit tab to add standard HTML tags automatically
2. Comments: use `Cmd-/` to comment out the current line
3. Link your JavaScript file: type `<sc` then tab. Edit "text/javascript" to the _relative_ path to your .js file (see below). I called mine `script.js`

JavaScript shortcuts in Sublime
1. type `fun` and hit tab to fill out the syntax of a JavaScript function:
    ```javascript
    function function_name(argument) {
    	// body...
    }
    ```

CSS shortcuts in Sublime  
1. There are none! Unless you install a package to autocomplete
2. (I do __not recommend installing this during the workshop__)
3. Here's a link: [Emmet] (https://packagecontrol.io/packages/Emmet)

__FYI: Understanding all this__  

- How to Git: https://guides.github.com/activities/hello-world/

__Presentation Slides__  
[Presentation Slides](https://docs.google.com/presentation/d/1H1J-vem8cPNo6lDoYmNzqXwnJ8cDNd7kBEQ8M50v6Z0/edit?usp=sharing)  
[W3Schools](https://www.w3schools.com/): Lots of easy webdev documentation
