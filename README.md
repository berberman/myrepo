# myrepo

Add the key to pacman keyring:

```
# wget -qO - https://raw.githubusercontent.com/berberman/myrepo/master/berberman.asc \
    | pacman-key --add -
```

You can check the fingerprint:

```
# pacman-key --finger C4F93F1ED397E8CF
```

Then sign it locally:

```
# pacman-key --lsign-key C4F93F1ED397E8CF
```

Append this repo in  `/etc/pacman.conf`:

```
[berberman]
Server = https://repo.typed.icu/$arch
```

