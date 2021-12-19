# Cracker blog

## Git setup in WSL

1. Copy the `.ssh` directory from Windows to WSL with `cp -r /mnt/c/Users/<user>/.ssh ~/.ssh`.
2. Add [keychain](https://www.funtoo.org/Keychain) with `sudo apt install keychain`.
3. Open or create `.bash_profile` file (you can do this by using VSC `code ~/.bash_profile`).
4. Add following line to the file (you might need to replace `id_rsa` to `id_ed25519` depending on your key):

```
eval `keychain --eval --agents ssh id_rsa`
```

## Tools setup in WSL:

1. Node.js - `sudo apt install nodejs`.
2. NPM - `sudo apt install npm`.
3. NPX - `sudo apt install npx`.