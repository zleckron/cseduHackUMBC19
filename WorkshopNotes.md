__We're doing everything fast, here are the notes__
- Download Sublime3: [sublime.com/3](https://www.sublimetext.com/3)
- Download Sublime Merge (for Git): [sublimemerge.com] (https://www.sublimemerge.com/)
- Clone _this_ repository: https://github.com/zleckron/cseduHackUMBC19.git

__In Sublime__
- Make a file and save it as `index.html` (the "index" part of the name is not very significant but the html file extension is)
- With your saved .html file open, type `<ht` then hit tab to add standard HTML tags automatically

_HTML Fast Facts!_
1. Pretty much everything in HTML is in _tags_ enclosed in an opening and closing tag with angle brackets!
    - Normal HTML tag to make a paragraph: `<p>literal string content</p>`
    - Tag to make a line break (doesn't ): `<br>`
  You can assume that most tags require a closing tag like `</p>` but there are exceptions like `<br>` to look out for
2. Strings don't need to go in quotes! See above paragraph example - the words "literal string content" will appear on the HTML page.

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
		<td>Hacker Floor</td>
	</tr>
</table>
```
_Making it look good_
- File > New or `Cmd-n` to make a new file, save it to styles.css (CSS style sheet) in the same folder as index.html
- CSS rule syntax:
- Color picker: [htmlcolorcodes.com](https://htmlcolorcodes.com/color-picker/)
- Photos that are safe to use: [Unsplash.com] (https://unsplash.com/)

_Making it do things_
- File > New or `Cmd-n` to make a new file, save it to .js (JavaScript)


__Testing__

__Uploading to Git__

__Programming Practices__
Accessibility
We want to encourage good programming practices. To make your website appealing to a variety of users, you should follow some compliance guidelines.
1. Article with an easy-to-understand list of ADA compliance website issues (I recommend you skip to the issues): https://www.digitalauthority.me/resources/ada-compliance-website/
2. Check for at least 4.5:1 ratio of color contrast: https://webaim.org/resources/contrastchecker/
3. Having good alternative text for images and descriptive link text is important!
    - Alt text in HTML image tags looks like this: `<img src="truegrit.jpg" alt="Chesapeake Bay Retriever True Grit, best mascot in Maryland">`
    - Descriptive link text looks like this: `<a href="https://www.hackumbc.org/">HackUMBC Home Page 2019</a>`

__Copyrights & Legal Stuff__
1. Credit photos! Even though you should be using photos that are free, it's courteous to credit the photographer

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
