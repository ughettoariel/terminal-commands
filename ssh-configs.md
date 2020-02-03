`ssh-keygen -t rsa -b 4096 -C "ughettoariel@gmail.com"`

`pbcopy < ~/.ssh/id_rsa.pub`

`ssh-add ~/.ssh/id_rsa`

`ssh -T git@github.com`

`cd ~/.ssh/`

`touch config`

`code config`

```
Host *
  AddKeysToAgent yes
  UseKeychain yes
  IdentityFile ~/.ssh/id_rsa
```

`ssh-add -K ~/.ssh/id_rsa`
