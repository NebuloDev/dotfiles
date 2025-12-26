# Terminals

Terminals are a surprisingly convoluted aspect of any Linux desktop.

They split into two aspects, shells, and emulators. Shells are the programs that interpret commands, while emulators are simply the UI for the shell.

## Shells

Most distros come with bash out of the box. While being widely accepted, it is rudamentary.

Much better options exist, like zsh, but my personal favorite for day-to-day usage is [Fish](https://fishshell.com/) [[Arch](https://archlinux.org/packages/extra/x86_64/fish/)]. It comes with autocomplete and a ton of nice quality of life features.

> CachyOS uses fish by default

Additionally, for a more polished experienced, I use a prompt engine called [oh-my-posh](https://ohmyposh.dev/) [[AUR](https://aur.archlinux.org/packages/oh-my-posh-bin)].

## Emulators

Personally, I'm a fan of drop-down terminal emulators, opposed to dedicated windows.

Here is a list of my personal go-to's, both windowed and drop-down:

- Konsole - KDE's default terminal emulator, a good to have [[Arch](https://archlinux.org/packages/extra/x86_64/konsole/)]
- Yakuake - The drop-down version of Konsole, uses same profiles [[Arch](https://archlinux.org/packages/extra/x86_64/yakuake/)]
- Ghostty - The most customisable one, possibly less performant [[Arch](https://archlinux.org/packages/extra/x86_64/ghostty/)]
    - As of v1.2, supports slide-in terminals

## Configuration

### Fish

Given that the aformentioned packages were used for installing fish, no additional setup is awfully needed.

`fish` and `exit` can be used to enter and exit the shell respectively.

To add fish as the default shell, execute the following:

```bash
chsh -s "$(command -v fish)"
```

Fish keeps a config file in `~/.config/fish/config.fish` for each user.

By default, it does output a welcome message, which can be suppresed, by either:

Entering the following command in the fish shell
```bash
set -U fish_greeting ""
```

Or, adding this line to the fish config file
```bash
set fish_greeting
```

### Oh My Posh

After installing Oh My Posh, your shell must be configured to use it.

The instructions for other shells can be found on their [website](https://ohmyposh.dev).

For Fish, add the following line to the end of the fish config (`~/.config/fish/config.fish`):

```
oh-my-posh init fish | source
```

Then reload the shell by restarting your terminal or running `exec fish`.

Oh My Posh also needs custom fonts with built-in icons to display it's themes properly, which can be installed with the following command:

```bash
oh-my-posh font install meslo
```

In this case, I'm installing the Meslo font, which includes the Nerd Font variant that contains the needed icons. More options can be found on the website.

Make sure to set this font up in your terminal emulator or system as this is usually not automatic.

> [!TIP]
> With the Meslo fonts, emulators often prefer the Propo versions over the Mono versions.

Lastly, Oh My Posh comes with themes, and a lot of them. The ones that come packaged with oh-my-posh can be found [here](https://ohmyposh.dev/docs/themes).

To use a theme (at least for fish), edit the line that you added into the config from `oh-my-posh init fish | source` to:

```
oh-my-posh init fish --config 'theme-path' | source
```

Replace `theme-path` with a path or link to the `.omp.json` file that you are using for the theme. For themes that come packaged with oh-my-posh, just the name of the theme without any pathing or file extensions is fine.

Currently I am using `blue-owl`.

### Konsole

The Konsole doesn't need pretty much any changes to the window itself, however some theming to it's profiles is nice.

In top right corner, the Konsole menu can lead to the settings dropdown which opens the "Configure Konsole" menu. In the profiles section, setup a new profile, and immediately head for the appereance tab.

This profile can be customised to your liking, but I like to use a modified version of the Campbell color scheme with the background for "Colour" and "Intense Colour" having the hex code `#232627`.

Any font changes, which are needed for Oh My Posh, are also to be done here.

Make sure to then set this new profile as the default in the general tab of the profile.

### Yakuake

> [!NOTE]
> The configuration in the Konsole section also applies here, using the "Configure Profiles" menu

Yakuake must be started manually, or added to the autostart in section in the KDE settings. It is treated as a regular application.

Afterwards, the Yakuake settings can be accessed by pressing F12, and clicking the burger menu, and then "Configure Yakuake"

In the Yakuake settings:

- Disabled "Show title bar" 
- Disabled "Open window after program start"
- Enabled "Show system tray icon" (For settings access)
- Theme: [Qogir Materia Dark](https://store.kde.org/p/2230336) (Available in KDE Store)

### Ghostty

Ghostty is super customisable, and all of its configuration can be found in one file, being `~/.config/ghostty/config`. By default it starts with a bunch of comments, but no actual configuration.

It's best to learn about ghostty's configuration through their [documentation](https://ghostty.org/docs), as I'm far too new to Ghostty for this, but I will leave my config in this folder as `ghostty-config`.

Ghostty typically works best and akin to the intended MacOS experience with KDE + Wayland, but more information can be found in the documentation or forums.