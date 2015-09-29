<p align="center">
  <img src="media/GreatWave.jpg" alt="swim logo" width = "400" />
  <br>
  <br>
  <p align = "center">
    <b>sw</b>itch v<b>im</b>rc files
  </p>
</p>

<br>
##Demo
show a gif of the usage here

<br>
##Install
Backup your files **before** swimming

```shell
curl -s https://raw.githubusercontent.com/dawsonbotsford/swim/master/install | bash
```

<br>
####Requirements
* node.js and npm

<br>
##Examples
```shell
  swim add https://raw.githubusercontent.com/dawsonbotsford/swim/master/exampleVimrcs/vimrcWikia.vim example
  swim ls                    #Show available swim aliases
  swim with example          #Set alias ```example``` as primary .vimrc
  swim with main             #Set alias ```main``` as primary .vimrc

```

<br>
##Available Commands
```shell
swim add <URLToRaw or pathToFile>  <alias>   #Add a swim alias
swim with <alias>                            #Change active vimrc file
swim ls                                      #List aliased vimrc files
swim active                                  #Show currently aliased vimrc
swim mv <alias1> <alias2>                    #Rename alias (like Linux mv)
swim rm <alias>                              #Delete an alias entirely
swim update                                  #Download newest version
swim version                                 #Print version
swim help                                    #Print this message
```

<br>
##Update
```shell
swim update       #Download newest version of swim
```

<br>
##Changelog
* **1.0.0**: Initial Launch
* **Prelaunch**: Beta Testing

<br>
##License
MIT
