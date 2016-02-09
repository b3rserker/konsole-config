# konsole-config
Configuration files for Konsole linux terminal emulator + specific mappings and overrides for some keys

# For brand new KDE5
export KENV=~/.kde/share/apps/konsole/

# For KDE5 created by migration from KDE4
export KENV=~/.kde4/share/apps/konsole/

# Quick access
!!! rm -rf $KENV

mkdir $KENV

ln -s $KENV ~/.konsole-config

cd ~/.konsole-config

git init

git remote add origin https://github.com/b3rserker/konsole-config

git config branch.master.remote origin

git config branch.master.merge refs/heads/master

git pull
