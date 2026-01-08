# Apps

The apps that I use on my systems and work incredibly well. The apps here don't have any complex setups or configurations unless explicitly stated. 

Certain apps/utilities or even entires sections can be in different areas instead of this list, mainly `/terminals`, `/gaming`, `/os`, as they are much more complicated topics due to the configuration required.

If browsing the Arch Repository, CachyOS repository, or AUR is too much, Pamac is a nice GUI application that handles both browsing and updates. Available both on [CachyOS Repository](https://packages.cachyos.org/package/cachyos/x86_64/pamac-aur) and [AUR](https://aur.archlinux.org/packages/pamac-aur).

## Internet

**Browsers**:
- [Zen Browser](https://zen-browser.app/) - A modern open-source Firefox fork [[CachyOS](https://packages.cachyos.org/package/cachyos/x86_64/zen-browser-bin), [AUR](https://aur.archlinux.org/packages/zen-browser-bin)]
- [Helium Browser](https://helium.computer/) - A simple privacy-focused chromium-based browser [[CachyOS](https://packages.cachyos.org/package/cachyos/x86_64/helium-browser-bin), [AUR](https://aur.archlinux.org/packages/helium-browser-bin)]
- [Firefox](https://www.firefox.com/en-US/) - The default open-source browser for Linux [[Arch](https://archlinux.org/packages/extra/x86_64/firefox/)]

**Extensions**:
- uBlock Origin - The best free ad-blocker out there [[Mozilla](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/)]
    - Comes pre-installed on Helium Browser
- Improve YouTube - Advanced YouTube customiser [[Mozilla](https://addons.mozilla.org/en-US/firefox/addon/youtube-addon/)]
- [Bitwarden](https://bitwarden.com/) - Password management and autofill [[Mozilla](https://addons.mozilla.org/en-US/firefox/addon/bitwarden-password-manager/)]
- Simple Translate - Inline text translator [[Mozilla](https://addons.mozilla.org/en-US/firefox/addon/simple-translate/)]
- 600% Sound Volume - Volume booster [[Mozilla](https://addons.mozilla.org/en-US/firefox/addon/600-sound-volume/)]
- PWAs for Firefox - Progressive Web App support [[Mozilla](https://addons.mozilla.org/en-US/firefox/addon/pwas-for-firefox/)]
    - This will a require the FirefoxPWA package [[Arch](https://archlinux.org/packages/extra/x86_64/firefoxpwa/)]
- Plasma Integration -  Browser control for KDE Plasma [[Mozilla](https://addons.mozilla.org/en-US/firefox/addon/plasma-integration/)]
- SteamDB - Advanced features for Steam [[Mozilla](https://addons.mozilla.org/en-US/firefox/addon/steam-database/)]
- User Agent Manager & Switcher - It's in the name [[Mozilla](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/)]

**Social Media & Messaging**:
- [Telegram](https://telegram.org/) - Official Telegram Desktop Client  [[Arch](https://archlinux.org/packages/extra/x86_64/telegram-desktop/)]
- [Discord](https://discord.com/) - Official Discord Desktop Client [[Arch](https://archlinux.org/packages/extra/x86_64/discord/)]
    - Vesktop - Modified discord client with better Linux support [[CachyOS](https://packages.cachyos.org/package/cachyos/x86_64/vesktop-bin), [AUR](https://aur.archlinux.org/packages/vesktop-bin)]
- Zapzap - Open source feature-rich client for WhatsApp [[AUR](https://aur.archlinux.org/packages/zapzap)]
- [Element](https://element.io/en) - Most advanced client for Matrix protocol [[Arch](https://archlinux.org/packages/extra/x86_64/element-desktop/)]

## Development

**Platforms**:
- [Visual Studio Code](https://code.visualstudio.com/) - Microsoft's JS-based IDE [[AUR](https://aur.archlinux.org/packages/visual-studio-code-bin)]
- [Unity](https://unity.com/) Hub - The official launcher for Unity editors [[AUR](https://aur.archlinux.org/packages/unityhub)]
    - PlasticSCM - Version control for Unity [[AUR](https://aur.archlinux.org/packages/plasticscm-client-gui)]
- Android Studio - Official development platform for Android apps  [[AUR](https://aur.archlinux.org/packages/android-studio)]

> [!NOTE]
> Unity engines typically work with Visual Studio instead of Visual Studio Code, but it can be achieved through careful setup. Some resources I found are from [Microsoft](https://code.visualstudio.com/docs/other/unity) themselves and the [Unity Forums](https://discussions.unity.com/t/resolved-vscode-and-editor-on-linux-what-happens-when-vscode-is-from-aur-and-unity-is-from-flathub/1658951).

**Utilities**:
- VirtualBox - Virtual machine management [[Arch](https://archlinux.org/packages/extra/x86_64/virtualbox/)]
    - During install, a host module will be requested, I recommend using the DKMS module [[Arch](https://archlinux.org/packages/extra/x86_64/virtualbox-host-dkms/)]
    - For most users, the guest additions ISO is very useful [[Arch](https://archlinux.org/packages/extra/any/virtualbox-guest-iso/)]
- OpenJDK - Java Development suite (more info on the [Arch Wiki](https://wiki.archlinux.org/title/Java#OpenJDK)) [[Arch](https://archlinux.org/packages/extra/x86_64/jdk-openjdk/)]
- NVM - Manager for different Node.js versions [[Arch](https://archlinux.org/packages/extra/any/nvm/)]
- Termius - Modern SSH and SFTP client [[AUR](https://aur.archlinux.org/packages/termius)]

> [!WARNING]
> NVM will not work on fish, instead use nvm.fish [[GitHub](https://github.com/jorgebucaran/nvm.fish)], which is designed specifically for fish, and available as a fish plugin. To download it, use the fish plugin manager fisher [[Arch](https://archlinux.org/packages/extra/any/fisher/)].

## Office

- Dolphin - KDE's file manager [[Arch](https://archlinux.org/packages/extra/x86_64/dolphin/)]
- Ark - KDE's archiving tool [[Arch](https://archlinux.org/packages/extra/x86_64/ark/)]
- [OnlyOffice](https://www.onlyoffice.com/) - Modern open-source Office suite [[CachyOS](https://packages.cachyos.org/package/cachyos/x86_64/onlyoffice-bin), [AUR](https://aur.archlinux.org/packages/onlyoffice-bin)]
- Xournal++ - Annotating/Note taking tool [[Arch](https://archlinux.org/packages/extra/x86_64/xournalpp/)]
- Merkuro - KDE's calendar/contacts/email suite [[Arch](https://archlinux.org/packages/extra/x86_64/merkuro)]
- [Obsidian](https://obsidian.md/) - Local-first markdown-based note taker [[Arch](https://archlinux.org/packages/extra/x86_64/obsidian/)]
- Okular - KDE's document viewer [[Arch](https://archlinux.org/packages/extra/x86_64/okular/)]
- [Nextcloud](https://nextcloud.com/) Desktop Client - It's in the name, syncs your Nextcloud files [[Arch](https://archlinux.org/packages/extra/x86_64/nextcloud-client/)]

> [!TIP]
> Merkuro applications can be integrated into the Plasma shells, the guide can be found in the `/kde/integrations` folder.

## Multimedia

**Graphics**:
- Inkscape - 2D graphics editor for SVG, PNG, etc. [[Arch](https://archlinux.org/packages/extra/x86_64/inkscape/)]
- Kolourpaint - KDE's paint drawing tool [[Arch](https://archlinux.org/packages/extra/x86_64/kolourpaint/)]
- Gwenview - KDE's image viewer [[Arch](https://archlinux.org/packages/extra/x86_64/gwenview/)]
- [Blender](https://www.blender.org/) - Open-source 3D editor [[Arch](https://archlinux.org/packages/extra/x86_64/blender/)]
    - [AUR](https://aur.archlinux.org/packages/blender-bin) version may provide better extension support

**Video**:
- [OBS Studio](https://obsproject.com/) - Video recording and streaming [[Arch](https://archlinux.org/packages/extra/x86_64/obs-studio/)]
    - The official OBS studio doesn't support browser sources, for browser support use the community packages [[CachyOS](https://packages.cachyos.org/package/cachyos/x86_64/obs-studio-browser), [AUR](https://aur.archlinux.org/packages/obs-studio-liberty)]
- Kdenlive - KDE's video editor [[Arch](https://archlinux.org/packages/extra/x86_64/kdenlive/)]
- [DaVinci Resolve](https://www.blackmagicdesign.com/products/davinciresolve) - Studio-grade video editing suite [[CachyOS](https://packages.cachyos.org/package/cachyos/x86_64/davinci-resolve), [AUR](https://aur.archlinux.org/packages/davinci-resolve)]
    - The AUR version requires manual intervention when updating, see the pinned comments on the AUR repo.
- Handbrake - Open source video transcoding tool [[Arch](https://archlinux.org/packages/extra/x86_64/handbrake/)]
- VLC - The most popular video viewing tool [[Arch](https://archlinux.org/packages/extra/x86_64/vlc/)]
- UxPlay - Use your computer as an AirPlay display/server [[AUR](https://aur.archlinux.org/packages/uxplay)]

**Audio**:
- Spotify - The most popular music streaming app [[Arch](https://archlinux.org/packages/extra/x86_64/spotify-launcher/)]
    - If you prefer spotify to NOT auto-update and handle them yourself, use the [[AUR](https://aur.archlinux.org/packages/spotify)] version instead.
- Helvum - Audio re-routing tool [[Arch](https://archlinux.org/packages/extra/x86_64/helvum/)]

## System Management

- Partion Manager - KDE's disk manager [[Arch](https://archlinux.org/packages/extra/x86_64/partitionmanager/)]
- GParted - GNOME's disk manager [[Arch](https://archlinux.org/packages/extra/x86_64/gparted/)]
- AMDGPU TOP - AMD GPU performance monitor [[Arch](https://archlinux.org/packages/extra/x86_64/amdgpu_top/)]
- LACT - GPU configuration and tuning tool [[Arch](https://archlinux.org/packages/extra/x86_64/lact/)]

## Other
- Caffeine-ng - Auto-sleep mode prevention [[AUR](https://aur.archlinux.org/packages/caffeine-ng)]
- KWrite - KDE's basic text editor [[Arch](https://archlinux.org/packages/extra/x86_64/kwrite/)]
- Spectacle - KDE's screenshot tool [[Arch](https://archlinux.org/packages/extra/x86_64/spectacle/)]
- [Bitwarden](https://bitwarden.com/) - Password management app [[Arch](https://archlinux.org/packages/extra/x86_64/bitwarden/)]
- KTailctl - GUI for Tailscale management [[AUR](https://aur.archlinux.org/packages/ktailctl)]
    - Needs the tailscale package [[Arch](https://archlinux.org/packages/extra/x86_64/tailscale/)]
- KDE Connect - KDE's device synchronisation app [[Arch](https://archlinux.org/packages/extra/x86_64/kdeconnect/)]

> [!NOTE]
> KDE Connect has interesting interactions across different devices and software. See more in the `/kde/integrartions` folder.
