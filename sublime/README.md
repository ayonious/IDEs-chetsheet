# SUBLIME TEXT:


## Install

Just google sublime text. download the installer for mac click on it.
	http://www.sublimetext.com/3
Try these to get little practice on sublime text
	http://code.tutsplus.com/articles/perfect-workflow-in-sublime-text-free-course--net-27293
	http://leveluptuts.com/tutorials/sublime-text-tutorials



## Useful shortcuts
	ctrl+P              to find a file
	ctrl+f 				find string in a file
	cmd+shift+f 		find string /regex in entire project


## Install the shortcut to open a directory in sublime from command line

Test
```
#goto a folder you want to open in sublime
/Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl .
```

If `Test` works you need to put that in the bin folder
```
cp /Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl /usr/local/bin/subl
```

Test Again:
```
#goto a folder you want to open in sublime
subl .
```

## Install package control in sublime: 
This is used to get some really cool plugins in sublime
	https://packagecontrol.io/installation

open sublime
view>show console>write the code that is in the above link and press enter> the package control should be installed

install the sublime plugin that will sunc between kvm and local machine, this will operate when you save the file
(make sure you are in same commit/branch in git for both.....)


How to install a package using package installer in sublime:
============================================================
cmd+shift+p > Package Control: install package (click) > now you will get list of all options <rsync ssh>
cmd+shift+p > Package Control: install package (click) > now you will get list of all options <git>



## How to use srync ssh:
1. 	Open the folder in a 'project' in sublime
2. 	When you open a project in sublime there will be a {name}.sublime-priject file created most probably in your Documents folder
3. 	now in sublime>project>edit project, a json file will open. now edit this file like this:
Sublime Settings file

NOW take a look at the "settings" part

change these according to your config

"remote_host": "off",
"remote_path": "/usr/local/git_tree/main",
"remote_user": "nkamal"


Now each time you save a file it will be copied to kvm 
:D :D :D



## Create snippet:
	http://sublimetext.info/docs/en/extensibility/snippets.html

```
<snippet>
  <!-- Example: Hello, ${1:this} is a ${2:snippet}. -->
  <content><![CDATA[
########### DEBUG REMOVE DEBUG REMOVE DEBUG REMOVE DEBUG REMOVE  ###########
use DDDATA::Dumpering;
########### DEBUG REMOVE DEBUG REMOVE DEBUG REMOVE DEBUG REMOVE  ###########
]]></content>
  <!-- Optional: Set a tabTrigger to define how to trigger the snippet -->
  <tabTrigger>dump</tabTrigger>
  <description>Add debug data::dumper line</description>
  <!-- Optional: Set a scope to limit where the snippet will trigger -->
  <scope>src.java, keyword.control.something</scope>
</snippet>
```