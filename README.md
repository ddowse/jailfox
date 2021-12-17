# Firefox
Bastille template to bootstrap Firefox and run it.

## Bootstrap
```shell
bastille bootstrap https://github.com/ddowse/jailfox
```

## Apply
```shell
bastille template TARGET ddowse/jailfox
```

## Adjust
```shell
bastille config TARGET set exec.start "/bin/sh /home/firefox/run-firefox"`
bastille config TARGET set exec.jail_user "firefox"

# See BastilleBSD Readme https://github.com/BastilleBSD/bastille#zfs-support for details about $bastille_prefix 
install $bastille_prefix/templates/ddowse/jailfox/jailfox /usr/local/bin/
install $bastille_prefix/templates/ddowse/jailfox/jail-firefox-exec /usr/local/libexec
```

## Run
```shell
xhost +local:
jailfox
```

