# Firefox
Bastille template to bootstrap Firefox.

## Description

When applied to a container, this template will   
   
 - install firefox,noto fonts package and helper utility
 - create a user named `firefox` 
 - will make the local X11 Socket available inside the jail.

To run the jailed firefox from the host system please visit 
[jailfox-install](https://github.com/ddowse/jailfox-install) for further instructions.

## Bootstrap
```shell
bastille bootstrap https://github.com/ddowse/jailfox
```

## Apply
```shell
bastille template TARGET ddowse/jailfox
```
