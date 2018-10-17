```sh
sudo scutil --set ComputerName "newname"

sudo scutil --set LocalHostName "newname"

sudo scutil --set HostName "newname"

```

I would add these last two steps.

> Flush the DNS cache by typing: dscacheutil -flushcache

> Restart your Mac.

