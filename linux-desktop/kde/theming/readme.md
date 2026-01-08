# KDE Theming

KDE is a very customisable DE, and capable of a lot. Unfortunately, I prefer a simple but finetuned UI, akin to Windows.

For my theming, I sometimes use a few specific tools:

- Kvantum for application theming [[Arch](https://archlinux.org/packages/extra/x86_64/kvantum/)]
- Klassy for window decorations [[AUR](https://aur.archlinux.org/packages/klassy-bin)]
- Panel colorizer for panel theming [[AUR](https://aur.archlinux.org/packages/plasma6-applets-panel-colorizer)]

I've compiled certain "presets" with time. These will guide the entire setup and used themes.

> [!NOTE]
> Most of these **are** available on the [KDE Store](https://store.kde.org/browse/), and hence downloadable directly from plasma.
> Breeze themes are pre-installed with KDE, no need to install those :)

### Modern Breeze (Current)

Themes: 
- [Breeze](github.com/KDE/breeze) as my plasma/global theme
- [Papirus](https://github.com/PapirusDevelopmentTeam/papirus-icon-theme) (Dark Variant) as my icon theme
- [Breeze](github.com/KDE/breeze) as my GTK theme
- [WinSur-dark-cursors](https://github.com/yeyushengfan258/WinSur-dark-cursors) as my cursor theme

Additional Applets:
- [PlasMusic Toolbar](https://github.com/ccatterina/plasmusic-toolbar)
- [kAirPods](https://github.com/can1357/kAirPods) (Optional)

Attached configuration files:
- Modern_Breeze.klpw (Klassy)

There are two panels, one at the bottom, which is full-width, floating, and always visible. Recommended height for both panels is 46px.

#### Bottom Panel
The bottom panel is very similar to standard Plasma 6 layout or Windows, with the standard KDE application launcher at the far left with the `view-grid` icon. The icons-only task manager should have small spacing between icons.

The digital clock is customised to only show the time with a Noto Sans bold font at 10px (can be different based on display) to match the height of the tray icons. The system tray can be customised to your liking.

Add panel colorizer and make sure the widget is hidden and cannot be configured from any other widget. Make sure in appearance that the panel updates on entering/exiting the floating state. The system tray icon replacer is a very useful tool.

#### Top Panel
This panel is for media controls. Create a floating, auto-hide, fit-content, centered panel with the PlasMusic applet in the middle, with the Bluetooth and kAirPods applets on the left and right respectively (optional). Don't forget to add panel colorizer.

Using panel colorizer, turn off the background of the panel and enable background and radius for the widgets themselves (radius 8). Ensure widget padding is 0 all around and the spacing of widgets is 4. If using the bluetooth and kAirPods widgets, shrink them by giving them a top and bottom margin of 8, through the preset overrides (kAirPods miscenters the icon so an extra margin of 1 on the left might be needed). I 

Lastly, configure the applets to your liking, I recommend setting both the panel and full view of the PlasMusic applet to use colors from the album cover as a background and allow the panel view to have full width if needed, all controls, album cover as icon, and media progress shown. In my opinion, the kAirPods icon looks better without the pulsing indicator.

### Fluent/Windows 10
- [Fluent-kde](https://github.com/vinceliuice/Fluent-kde) (Dark Variant) as my plasma/global theme
- [Colloid-icon-theme](https://github.com/vinceliuice/Colloid-icon-theme) (Bold Dark Variant) as my icon theme
- [Fluent-gtk](https://github.com/vinceliuice/Fluent-gtk-theme) (Dark Variant) as my GTK theme
- [WinSur-dark-cursors](https://github.com/yeyushengfan258/WinSur-dark-cursors) as my cursor theme

No guide available here, some imagination might be required. I do reccomend using kvantum to integrate Fluent-Kde into applications properly.