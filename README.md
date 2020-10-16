# myrepo

Add the key to pacman keyring:

```bash
wget -qO - https://raw.githubusercontent.com/berberman/myrepo/master/berberman.asc \
    | sudo pacman-key --add -
```

Append this repo in  `/etc/pacman.conf`:

```
[berberman]
Server = https://repo.typed.icu/$arch
```

