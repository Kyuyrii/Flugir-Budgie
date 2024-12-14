Flugir Budgie is a theme for the Budgie desktop, based on the Qogir theme.

It also comes with the FlugirDot cursors, based on the GoogleDot cursors.

To use it in Snap applications, you need to install the Snap version of the theme.

<a href="https://snapcraft.io/flugir-budgie-theme">
  <img alt="Get it from the Snap Store" src="https://snapcraft.io/en/dark/install.svg" />
</a>

Currently, you also need to use these 2 commands to connect the theme with the currently installed applications, reusing the commands if you install new applications.

``` for i in $(snap connections | grep gtk-common-themes:gtk-3-themes | awk '{print $2}'); do sudo snap connect $i flugir-budgie-theme:gtk-3-themes; done ```

``` for i in $(snap connections | grep gtk-common-themes:icon-themes | awk '{print $2}'); do sudo snap connect $i flugir-budgie-theme:icon-themes; done ```

Here are the links to the projects I used to create the Flugir theme:

Qogir theme: https://github.com/vinceliuice/Qogir-theme

GoogleDot cursors: https://github.com/ful1e5/Google_Cursor

Fluent theme: https://github.com/vinceliuice/Fluent-gtk-theme
