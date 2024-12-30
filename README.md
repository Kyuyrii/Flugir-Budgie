Flugir Budgie is a theme for the Budgie desktop, based on the Qogir theme.

It also comes with the FlugirDot cursors, based on the GoogleDot cursors.

If you want to install the latest version via terminal, just use this command:

``` wget https://github.com/Kyuyrii/Flugir-Budgie/releases/download/Flugir-Budgie-0.7/WFB-0.7.zip && unzip WFB-0.7.zip && ./FBF-0.7/IFB.sh ```

![Snapshot_2024-12-18_05-37-01](https://github.com/user-attachments/assets/b45f5cf0-be63-4afb-8d59-f7eb9be1facf)

I recommend using the Papirus icons, so I added them to the Flugir Budgie installation script.

To use it in Snap applications, you need to install the Snap version of the theme.

<a href="https://snapcraft.io/flugir-budgie-theme">
  <img alt="Get it from the Snap Store" src="https://snapcraft.io/en/dark/install.svg" />
</a>

Unfortunately, you still need to use these commands to use the theme in installed Snap applications.
And reuse them when installing new Snap applications.

``` for i in $(snap connections | grep gtk-common-themes:gtk-3-themes | awk '{print $2}'); do sudo snap connect $i flugir-budgie-theme:gtk-3-themes; done && for i in $(snap connections | grep gtk-common-themes:icon-themes | awk '{print $2}'); do sudo snap connect $i flugir-budgie-theme:icon-themes; done ```

Here are the links to the projects I used to create the Flugir theme:

Qogir theme: https://github.com/vinceliuice/Qogir-theme

GoogleDot cursors: https://github.com/ful1e5/Google_Cursor

Fluent theme: https://github.com/vinceliuice/Fluent-gtk-theme

Arc theme of Ubuntu repository.
