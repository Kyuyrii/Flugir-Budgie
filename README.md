# Flugir Budgie

Flugir Budgie is a theme for the Budgie desktop, based on the Qogir theme.

It also comes with FlugirDot cursors, based on GoogleDot cursors, and Flugir-Tela icons, a slight modification of Tela-nord-dark.

If you want to install version 0.9.3 via terminal, use the command below, I recommend restarting the system after the installation is complete.

``` wget https://github.com/Kyuyrii/Flugir-Budgie/releases/download/Flugir-Budgie-0.9.3/WFB-0.9.3.tar.xz && tar -xf WFB-0.9.3.tar.xz && ./FBF-0.9.3/IFB.sh ```

![Snapshot_2025-01-06_03-21-43](https://github.com/user-attachments/assets/02238dca-4c01-4dae-a183-9820ec87a65e)

To use it in Snap applications, you need to install the Snap version of the theme.

<a href="https://snapcraft.io/flugir-budgie-theme">
  <img alt="Get it from the Snap Store" src="https://snapcraft.io/en/dark/install.svg" />
</a>

Unfortunately, you still need to use this command to theme installed Snap apps.
And reuse them when installing new Snap apps.

``` for i in $(snap connections | grep gtk-common-themes:gtk-3-themes | awk '{print $2}'); do sudo snap connect $i flugir-budgie-theme:gtk-3-themes; done && for i in $(snap connections | grep gtk-common-themes:icon-themes | awk '{print $2}'); do sudo snap connect $i flugir-budgie-theme:icon-themes; done ```

# These were the projects I used to make the Flugir Budgie theme.

Qogir:

https://github.com/vinceliuice/Qogir-theme

https://github.com/vinceliuice/Qogir-icon-theme/tree/master/src/cursors

Matcha:

https://github.com/vinceliuice/Matcha-gtk-theme

Arc theme of Ubuntu repository.

Papirus:

https://github.com/PapirusDevelopmentTeam/papirus-icon-theme

Tela:

https://github.com/vinceliuice/Tela-icon-theme

GoogleDot cursors:

https://github.com/ful1e5/Google_Cursor
