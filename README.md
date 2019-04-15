<p align="center">
  <img src="media/GreatWave.jpg" alt="swim logo" width = "400" />
  <br>
  <br>
  <p align = "center">
    <b>sw</b>itch v<b>im</b>rc files instantly
    <br><br>

    
  </p>
</p>
<br>
    
![](https://img.shields.io/badge/version-0.4.0-brightgreen.svg)
![](https://img.shields.io/badge/license-MIT-blue.svg)

## Demo
![demo fig](media/demo.gif)

<br>

## Why
Trying out and switching vimrc's shouldn't be hard. It shouldn't require several ```mv```'s combined with a ```wget```. Most importantly, it shouldn't stop you from always having the perfect vim configuration so you can be efficient. 
<br>
<p align="center">
  <b><code>swim add</code> vimrc's directly from the internet</b>
</p>
or locally and alias your vimrc's with names that are easy to remember. Swim entirely replaces the need for per-directory vimrc's, headers, and external vimrc configs.

<br>

## Install
Backup your files **before** swimming

```shell
curl -s https://raw.githubusercontent.com/dawsonbotsford/swim/master/install | bash
```

<br>

## Examples

```shell
  swim add ~/dotfiles/myVimrc favorite    #Add new swim alias
  swim ls                                 #Show available swim aliases
  swim add https://raw.githubusercontent.com/dawsonbotsford/swim/master/exampleVimrcs/vimrcWikia.vim example
  swim with favorite         #Set alias favorite as primary .vimrc
  swim with main             #Set alias main as primary .vimrc

```

<br>

## Update

```shell
swim update       #Update to the newest version of swim
```

<br>

## Available Commands

```shell
swim add <URLToRaw or pathToFile>  <alias>   #Add a swim alias
swim with <alias>                            #Change active vimrc file
swim ls                                      #List aliased vimrc files
swim active                                  #Show currently aliased vimrc
swim vim <alias>                             #Edit the vimrc stored at alias

swim mv <alias1> <alias2>                    #Rename alias (like Linux mv)
swim rm <alias>                              #Delete an alias entirely
swim update                                  #Download newest version
swim version                                 #Print version
swim help                                    #Print this message
```

<br>

## FAQ

* Where does swim store my vimrc files?
  * swim stores your vimrc files in ```~/.swim```. You can edit the vimrc files with ```swim vim <alias>``` or edit them manually from their file location.

<br>

*  Can I set a custom executable location?
  * Yes, the default install location of the `swim` executable is `/usr/local/bin`, but if you would like a custom location, simply set the environmental variable named `usrDir`. 
  * Example: `export usrDir="/usr/sbin"`
(That only needs to be set for when you perform the swim install. So no need to set this in your bashrc or zshrc)

<br>

* Does swim support emacs?
  * No, but pull requests are always welcome :)

<br>

* Can I call swim within vim?
  * It may be possible to hack together a several command ```:! ``` solution at the moment, but there is not a supported method.
  
<br>

#### Requirements

* node.js and npm (to auto-install [chalk-cli](https://github.com/chalk/chalk-cli))

<br>

## Changelog

* **0.4.0**: Custom executable install location
* **0.3.2-prelaunch**: Prelaunch Beta Testing
