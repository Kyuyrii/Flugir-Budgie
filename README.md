# Flugir Budgie

Flugir Budgie is a theme for the Budgie desktop, based on the Qogir theme.

It also comes with the FlugirDot cursors, based on the GoogleDot cursors, and Papirus icons using Papirus Yaru folders.

If you want to install the version 0.7.1 via terminal, just use this command:

``` wget https://github.com/Kyuyrii/Flugir-Budgie/releases/download/Flugir-Budgie-0.7.1/WFB-0.7.1.zip && unzip WFB-0.7.1.zip && ./FBF-0.7.1/IFB.sh ```

![Snapshot_2024-12-18_05-37-01](https://github.com/user-attachments/assets/b45f5cf0-be63-4afb-8d59-f7eb9be1facf)

To use it in Snap applications, you need to install the Snap version of the theme.

<a href="https://snapcraft.io/flugir-budgie-theme">
  <img alt="Get it from the Snap Store" src="https://snapcraft.io/en/dark/install.svg" />
</a>

Unfortunately, you still need to use this command to theme installed Snap apps.
And reuse them when installing new Snap apps.

``` for i in $(snap connections | grep gtk-common-themes:gtk-3-themes | awk '{print $2}'); do sudo snap connect $i flugir-budgie-theme:gtk-3-themes; done && for i in $(snap connections | grep gtk-common-themes:icon-themes | awk '{print $2}'); do sudo snap connect $i flugir-budgie-theme:icon-themes; done ```

These were the projects I used to make the Flugir Budgie theme.

Qogir theme:

https://github.com/vinceliuice/Qogir-theme

GoogleDot cursors:

https://github.com/ful1e5/Google_Cursor

Fluent theme:

https://github.com/vinceliuice/Fluent-gtk-theme

Arc theme of Ubuntu repository.

Papirus:

https://github.com/PapirusDevelopmentTeam/papirus-icon-theme

https://github.com/PapirusDevelopmentTeam/papirus-folders
