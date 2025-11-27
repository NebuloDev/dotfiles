# Linux Desktop

> [!IMPORTANT]
> I'm no professional or voice of reason, this is just me writing down what Linux tools worked for me.

My personal guides for a nice optimal linux desktop setup with configuration files.

The majority of this folder is built around my optimal experiences on Linux, prioritising flexible development, customisation, and performant gaming on AMD hardware.

After trying several distro flavors, delving into a variety of package management option, desktop environments, etc, I've settled on a nice modern stack that has exceeded any experiences I had on Windows 10/11.

Get started with the `/os` folder to setup your system.

## Note on Package Management

My package management experiences with `snap`, `apt`, `rnf`, `flatpak` have all come with their shortcomings, and I absolutely love `pacman` (personal bias). Have heard good things about what NixOS uses though.

Hence I've fully switched to Arch or it's derivatives like CachyOS or EndeavourOS. For this reason, any packages listed in the readme's were installed through `pacman` or `yay`/`paru`, and the repositories used are either [Arch's Official Repository](https://archlinux.org/packages/), [CachyOS's Package Repository](https://packages.cachyos.org/), and the [Arch User Repository](https://aur.archlinux.org/packages).

Additionally, a personal choice is a prefer pre-built binary files for application instead of compiling myself. I know its less safe, but I prefer the convenience over the risk. Just be aware the package links do use the pre-packaged version whenever possible.

> [!WARNING]
> The Arch User Respository (AUR) is community managed! Install packages at your own risk. Make sure to only install packages you trust.