## iPhone Sync Location (?)

`/Users/[username]/Pictures/iPhone Library.photolibrary`

## Uninstalling Mac Apps

* https://discussions.apple.com/thread/3766698?start=0

> Very basically and generally you can, at the minimum, trash the application, prefPane, or whatever it is you want to
> uninstall. But you should be aware of some other details:
>
> 1. Apps may install *login* items or other *startup* items. Hopefully the ones that install other startup items will also
> supply their own uninstallers. Use the third party uninstaller whenever possible if it is supplied.
>
> 2. *Preferences* are usually stored in `~/Library/Preferences` generally as `.plist` files. You could, if you can't identify
> the plist file just leave it alone. If there is no program to use it the plist is just taking up space.
>
> 3. Many apps also can create stuff in `~/Library/Application Support`. Like the preferences these to could be ignored.
>
> 4. Like 2 and 3, some apps might use `~/Documents`, `~/Movies`, etc.
>
> 5. Apps installed with `.[m]pkg` installers usually will install their apps into `/Applications`. But except for stupid
> authors who for some odd reason want to supply their apps with .pkg installers where it only installs a single application,
> `.[m]pkg`'s will usually "spray" other stuff into your system into any of the places I mentioned previously but also may
> install into system level places if they request the admin password. Hopefully these installers will also supply some
> kind of uninstaller, either installed as part of the installation or supplied separately.

* http://osxdaily.com/2011/06/20/uninstall-mac-applications/
* http://www.thexlab.com/faqs/uninstallingapps.html

## updatedb

* http://superuser.com/questions/109590/whats-the-equivalent-of-linuxs-updatedb-command-for-the-mac

`sudo /usr/libexec/locate.updatedb`
