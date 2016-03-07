# JW Player Support Team Reproduction Page

### Table of Contents
***
[Getting Started](#getting-started)  
[Features](#features)  
[Page Setup](#page-setup)  
[Formatting](#formatting)  
[Issues? Feature Requests?](#issues-feature-requests)  
[Acknowledgements](#acknowledgements)

### Getting Started
***
If you want to download the source code, you can do so from this GitLab repository by clicking on the download button above.  

However, if you use TextExpander, I would recommend copying and pasting the contents of [demo-uikit.html](https://gitlab.com/waxidiotic/jw-demo/blob/master/demo-uikit.html) into a new snippet. This way you can easily create a new reproduction page by expanding the snippet inside of a new document in your text editor of choice.  

There is no need to download any of the JavaScript or CSS referenced by this reproduction page as they are all linked to using absolute URLs.

### Features
***
The page has a 640 x 360 player embedded on it. Also on the page, below the player, are the following tabs:  
  
* **Browser & Reproduction** (hideable, if not for an escalation)  
* **Description** (hideable, if for an escalation)  
* **Player Details** - shows the player version, rendering mode, media format, and playlist item
* **Player Log** - This tab shows the output of the `.on('all')` API event.
  
### Page Setup
***
By default, the page is setup in a way that is well-suited for escalations and bug reports.  
  
If you would like to change this behavior to be more of a demo page, all you would need to do is comment and uncomment some lines of the code.  
  
* Escalations/Bug Reports
	* Lines That Need to be Uncommented
		* 29
		* 43 thru 58
	* Lines That Need to be Commented
		* 30
		* 63 thru 65  
  
* Demo Pages
	* Lines That Need to be Uncommented
		* 30
		* 63 thru 65
	* Lines That Need to be Commented
		* 29
		* 43 thru 58  
  
To easily comment and uncomment code, most text editors support a keyboard shortcut. Just select whatever code you would like to be affected and press CMD+/ (forward-slash) on Mac or CTRL+/ on Windows.

### Formatting
***
**Alert**  
  
`<div class='uk-alert'>Text of the Alert</div>`  
  
**Inline Code**  
  
`<code>playerInstance.play();</code>`
  
**Code Section**
  
	<pre>
	  <code class='lang-js'>
	    playerInstance.setup({  
	      file: 'whatever.mp4'
	    });
	  </code>
	</pre>
  
The class attribute of the `<code>` tag can be set to a different scripting language. The example above is set to highlight code syntax for JavaScript. If you would want to change it to HTML or CSS, you can change the class name to `lang-html` or `lang-css`, respectively.

### Issues? Feature Requests?
***
Have an issue or a feature request? Create a new issue on this project's [GitLab repository](https://gitlab.com/waxidiotic/jw-demo/issues).

### Acknowledgements
***
* [Highlight.js](https://github.com/isagalaev/highlight.js), for syntax highlighting - &copy; 2016 Ivan Sagalaev
* [UIkit](http://www.getuikit.com), CSS framework - &copy; 2016 YOOtheme
