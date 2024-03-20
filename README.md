# keepassxc-cr-recovery.html

A small tool that helps you regain access to your KeePassXC password database in case 
you have it protected with YubiKey challenge-response and lost your key --
Now comes with HTML so you can run it virtually everywhere.

Currently supports KDBX4 databases with Argon2 hashing.

## Usage

What you need:
* your KeePassXC database
* your challenge-response secret. This cannot be retrieved from the YubiKey, it needs to be saved upon initial configuration of the key.

Then just save the html anywhere, open it with a browser, and feed them into it.
You will get a keyfile downloaded.
Then, to unlock your database in KeePassXC, you need to check "key file" instead of "challenge response" and load the file.

## Credits

Basically a translation of the official [keepassxc-cr-recovery](https://github.com/keepassxreboot/keepassxc/blob/develop/utils/keepassxc-cr-recovery/README.md) into HTML/JS.

Special thanks to [@gilcu3](https://github.com/gilcu3) for this [comment](https://github.com/keepassxreboot/keepassxc/issues/1734#issuecomment-1948641668).

Licensed in GPLv3 because it's a derivative of kpXC which is GPLv3.
