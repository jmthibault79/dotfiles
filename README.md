I like to keep my system files AKA "dot files" in sync between my devices.
They are all MACS with BASH shells, so a lot of this probably won't work if this doesn't describe your environment.
There are probably some unknown-unknowns that depend on my personal setup too.  No guarantees!

Some of my files have private and public components (like .profile and .aliases).
I keep the private version in my homedir, and use a softlink to the public version in my dotfiles.

Example:
```
ln -s ~/src/dotfiles/.aliases-public .
```

To combine them, my private version starts with a line like this:
```
source .aliases-public
```
