# WOLWizard: The Wake-on-LAN wizard
A tool to send WOL packets using a user-friendly TUI interface

## Dependencies
- A POSIX-compatible shell
- `dialog` or `whiptail` (The latter is pre-installed on Debian/Ubuntu)
- [`wakeonlan`](https://github.com/jpoliv/wakeonlan/): This is intended to be replaced with a custom implementation in the future 
  - Package `wakeonlan` in the [Debian](https://packages.debian.org/search?keywords=wakeonlan)/[Ubuntu](https://packages.ubuntu.com/search?keywords=wakeonlan) repositories
  - Package [`wakeonlan`](https://archlinux.org/packages/extra/any/wakeonlan/) in the AUR
  - Package [`net-misc/wakeonlan`](https://packages.gentoo.org/packages/net-misc/wakeonlan) for Gentoo
  - Nixpkg [`wakeonlan`](https://search.nixos.org/packages?show=wakeonlan)

## Installation
```sh
sudo make install
```

## Configuration
The environment variable `WOLWIZARD_DIALOG` can be used to override the dialog command used, when unset `dialog` will be used, if `dialog` isn't available, `whiptail` will be used as a fallback

## Images
![Main screen](img/mainscreen.png) Main screen
![MAC address entry](img/macentry.png) MAC address entry
