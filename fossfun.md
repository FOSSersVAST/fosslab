# Fun things you can do..

This tutorial show how much fun is foss..(This sentence doesn't make any sense at all :\ )

## Figlet

Figlet is an amazing CLI tool which helps in displaying amazing fonts in your terminal :)

First check whether ``figlet`` is installed in your system. 
```bash
$ sudo apt-get install figlet
```

Try using figlet by doing..
```bash
figlet "Hello World!"
```
You can customize the font by using ``-f`` parameter.
```bash
figlet -f min "Awesome"
```

You can also extend the customization by many parameters. For knowing more, do
```bash
man figlet
```

_**BONUS**_ : Add ``lolcat`` and make it colourful!!
To use lolcat, you need to install it by
```bash
gem install lolcat
```

```bash
figlet -f 3d "This lit!!" | lolcat
```
The 3d.flf file is not installed predefault and can be used by copying into into ``\root\usr\share\figlet\`` folder.
Source to 3d.flf and other amazing custom figlet fonts : https://github.com/xero/figlet-fonts (Shoutout to xero, an amazing ricer)
