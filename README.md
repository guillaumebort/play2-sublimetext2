# A Play 2.0 Bundle for Sublime text 2

Get the latest Sublime Text 2 beta from http://www.sublimetext.com/2.

## Currently supported features

### Syntax highlighting

- For `*.scala.html`
- For `*.routes`
- For `*.conf`

### Code snippets

- `action ➝` : Creates an action (scala & java)
- `actor ➝` : Get an actor from Akka (scala & java)
- `aync ➝` : Creates an async result (scala & java)
- `bindform ➝` : Creates form binding from request structure (scala & java)
- `cacheget ➝` : Retrieve value from cache (scala & java)
- `cacheset ➝` : Put value in cache (scala & java)
- `callbackenum ➝` : Creates callback enumerator (scala)
- `controller ➝` : Creates a Controller structure (scala & java)
- `dbconn ➝` : Creates a DB.withConnection structure (scala & java)
- `dbtrans ➝` : Creates a DB..withTransaction structure (scala & java)
- `entity ➝` : Creates a Ebean entity structure (java)
- `evolutions ➝` : Creates the evolution up/down tags in sql file
- `pforeach ➝` : Creates an foreach structure in templates (html)
- `form ➝` : Creates a simple form structure (scala & java)
- `pform ➝` : Creates a simple html form (html)
- `fromconf ➝` : Creates value from conf file (scala & java)
- `global ➝` : Creates a Global object structure (scala & java)
- `htmlform ➝` : Creates a form in templates (html)
- `model ➝` : Creates a JDBC model structure (scala)
- `ok ➝` : Creates a Ok result (scala & java)
- `pushenum ➝` : Creates an imperative enumerator (scala)
- `redirect ➝` : Creates redirection (scala & java)
- `schedule ➝` : Creates a scheduled task (scala & java)
- `sql ➝` : Creates a SQL structure (scala)
- `sessionget ➝` : Retrieve a value from session (scala & java)
- `sessionset ➝` : Put value in session (scala & java)
- `sse ➝` : Creates a SSE action (scala)
- `tupleform ➝` : Creates a multiple input form (scala)
- `template ➝` : Creates a html template structure (html)
- `websocket ➝` : Creates a websocket action (scala & java)

## Theme

Currently optimized for the __Dawn__ theme.

## Installation instructions : 

### Cross Platform Via [Sublime Package Control](http://wbond.net/sublime_packages/package_control)

Click: 
    
    Tools > Command Palette...

Type:
    
    Install Package
    Play 2.0

### Mac 

    $ cd ~/Library/Application\ Support/Sublime\ Text\ 2/Packages/
    $ git clone git://github.com/guillaumebort/play2-sublimetext2.git play2
    
### Linux (Ubuntu like distros)

    $ cd ~/.config/sublime-text-2/Packages/
    $ git clone git://github.com/guillaumebort/play2-sublimetext2.git play2

### Windows 7:

    Copy the directory to: "C:\Users\<username>\AppData\Roaming\Sublime Text 2\Packages"

### Windows XP:

    Copy the directory to: "C:\Documents and Settings\<username>\Application Data\Sublime Text 2\Packages"

## Zen Coding tab completion in *.scala.html

Add the scope `text.play` to the comma separated list under the expand_zen_abbreviation_on_tab key binding in the ZenCoding `Default.sublime-keymap`:

    ...
    {
    "keys": ["tab"], "command": "expand_zen_abbreviation_on_tab", "context":
	[
		{ "key": "selector", "operator": "equal", "operand": "text.play, source.css - source.css.embedded, text.xml, text.xsl, text.html -source -meta.tag, meta.scope.between-tag-pair.html -source", "match_all": true },
    ...

in `Packages/ZenCoding/Default.sublime-keymap`
