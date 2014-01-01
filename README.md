## LogicIO RTCU - VPL Language Support for Sublime Text

This adds Syntax Definitions for the VPL programming language used
in LogicIOs RTCU software.

At the moment it has all the functions and reserved keywords from [RTCU IDE](http://www.logicio.com/HTML/index.html). Something to look at in the future could be custom functions and function signatures if needed.

### Installation
First navigate to the `Package` directory.

* **Windows**: %APPDATA%\Sublime Text 2\Packages
* **OS X**: ~/Library/Application Support/Sublime Text 2/Packages
* **Linux**: ~/.Sublime Text 2/Packages

Then checkout the project from github

```
git clone git@github.com:Springworks/VPL-Sublime.git VPL
```

Restart sublime. Now you should have the option for syntax highlight under

```
view -> Syntax -> VPL (LogicIO RTCU)
```

### Recompilation
To recompile files in the project you need [AAAPackageDev](https://github.com/SublimeText/AAAPackageDev). After that you can change the build system in Sublime Text 2 to `Convert To...`.

The file you want to change when updating the Syntax Definitions is
`vpl.YAML-tmLanguage` **not** `vpl.tmLanguage`. The YAML-file is the source and the tmLanguage-file is the compiled one.

### TODO

* Add snippets for regularly used pieces of code.
* Figure out how to auto detect the syntax based on file ending for .inc files.
* Add make file so we can recompile the .tmLanguage-files.
* Clean up the scopes after [Text Mates Naming Conventions](https://manual.macromates.com/en/language_grammars#naming_conventions)


### Links

* [Regexper](http://www.regexper.com/) - Visual aid for Regex.
* [AAAPackageDev](https://github.com/SublimeText/AAAPackageDev) - Development tool in Sublime.
* [RTCU IDE](http://www.logicio.com/HTML/index.html) - Language Reference
* [Syntax Defs](http://sublime-text-unofficial-documentation.readthedocs.org/en/sublime-text-2/reference/syntaxdefs.html) - Documentation for creating syntax defs
* [Syntax Defs 2](http://sublime-text-unofficial-documentation.readthedocs.org/en/sublime-text-2/extensibility/syntaxdefs.html) - Documentation for creating syntax defs 2