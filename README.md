# WARSAW Archlinux package

This is based on aur-warsaw-itau https://github.com/paulodiovani/AUR-warsaw-itau

Main credits goes to Paulo Diovani. This is just an adaption for BB based 
on his work for Itau

This package install the warsaw module for BB software libs and daemon on an 
[Archlinux][1] system.

This is the GAS module to access Banco do Brasil. It'll probably not work with other
banks but you can find the .deb files at http://www.dieboldnixdorf.com.br/warsaw

This is confirmed working with firefox and not working with google-chrome.

:warning: Notice that this package does not includes any software. All files
are downloaded from original sources during build process.

## Installing

```console
git clone https://github.com/ticianolage/aur-warsaw-bb.git warsaw
cd warsaw
makepkg -Acs
sudo pacman -U warsaw-0.1-1-x86_64.pkg.tar.gz
```

You may want to start/enable the service with.

```console
systemctl enable warsaw
systemctl start warsaw
```

[1]: https://www.archlinux.org
[2]: http://www.gastecnologia.com/suporte/warsaw
[3]: https://www.bb.com.br

