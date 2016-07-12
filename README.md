WukanacPhpSimpleRefactor for Sublime Text
===========

A simple way to integrate [PHP Refactoring Browser]'s method extraction in Sublime Text 3 

---

Requirements
===========
You need to have PHP installed and [PHP Refactoring Browser]'s refactor.phar file. 

Installation
=======
The package is available on [Package Control](https://sublime.wbond.net/).

Configuration
=======
Edit the file WukanacPhpSimpleRefactor.sublime-settings (Preferences > Package Settings > WukanacPhpSimpleRefactor > Settings – User) with the correct php_path and refactor_path.

Example:
	
	/** FILE: WukanacPhpSimpleRefactor.sublime-settings **/

	{
		"php_path" : "/Applications/MAMP/bin/php/php5.5.3/bin/PHP",
		"refactor_path" : "/usr/local/bin/refactor",
		"patch_path" : "patch",
		"patch_opts" : "--binary",
	}

Usage
=====
There are two functionalities:

**Extract method:** Select the lines that you'd like to extract to a new method, and use the shortcut **ctrl+alt+r** (or right click on the text and select "**WukanacPhpSimpleRefactor -> Extract method**"). The plugin will ask you for the method name to use. 

**Rename local variable:** Right click inside the scope that contains the local variable that you want to rename and select "**WukanacPhpSimpleRefactor -> Rename local variable**". The plugin will ask you for the variable old name and the new name.


License
----

MIT

[PHP Refactoring Browser]:https://github.com/QafooLabs/php-refactoring-browser
