# Run macOS Apps without any problem with admin privileges and GateKeeper



Some applications you download are not from appstore or maybe some of them are handmade with no Apple ID confirmed, so at this point we need some tricks

We have two tricks for this, I mean like Linux guys **macOS is UNIX** based operation System so you must work with terminal

Lest begin.

## Trick One

At the default view in **Settings** and **Security & Privacy** and in **General** Tab under section **Allow Apps downloaded from :** —>

There is just two option :

1. App Store
2. App Store and Identified Developer

So this command reveal another option in there :

```sh
$ : sudo spctl --master disable
```

After this :

```sh
$ : sudo spctl --status
```

Can show you stat of gatekeeper

And after runnig your application you can return in to ON

```sh
$ : sudo spctl --master-enable
```

DONE



## Trick Two

There is some other application that even if gatekeeper is disabled but macOS dont allow you to run it

These application are most hacking keygen cracking and other these type of apps

There is one command that can help you :

```sh
$ : xattr -c [PATH OF APP]
Example :
$ : xattr -c /Applications/BetterZip.app
```

After ENTER,this command , some plists and info from app content about developers and where you downloaded removed this make this app runable.

Also this is a answer from stack apple exchange forum who answer this as same as me :

To do this without needing admin privileges and without disabling security features:

- Open up terminal
- Type `xattr -c`
- Drag (from finder) the file you wish to open into the terminal window
- Run the command by pressing Enter

`xattr -c` removes the metadata of a file or folder. This removes the developer, date of download and a few other things. It does not effect the contents of the app.



Thanks for reading

