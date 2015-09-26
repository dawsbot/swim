<p align="center">
  <img src="img/GreatWave.jpg" alt="swim logo" width = "400" />
  <br>
  <br>
  <h3 align = "center">
    <b>sw</b>itch v<b>im</b>rc files inline instantly
  </h3>
</p>

<br>
##Demo
show a gif of the usage here

##Install
```shell
curl -s https://raw.githubusercontent.com/dawsonbotsford/swim/master/install | bash
```

##About
```shell
Usage:
  swim help                         #Show this message
  swim with <alias>                 #Change active vimrc file
  swim add <pathToFile> <alias>     #Add a swim alias
  swim ls                           #List aliased vimrc files
  swim active                       #Show currently aliased vimrc

Example:
  swim with main                               #Set ~/.swim/.swimrc.main to be your primary .vimrc
  swim with pairing                            #Set ~/.swim/.swimrc.pairing to be your primary .vimrc
  swim add ~/dot/.vimrcForPairing pairing      #Add an alias called pairing

```
Keeping your main vimrc file anywhere besides ``` ~/.swim/swimrc.main``` is **not** supported.


*Backup your dotfiles often and before swimming. I am not responsible for any loss of data.*
