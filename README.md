Flugir Budgie is a theme for the Budgie desktop, based on the Qogir theme.

It also comes with the FlugirDot cursors, based on the GoogleDot cursors.

I recommend using the Papirus icons, so I added them to the Flugir Budgie installation script.
But I also included the icons that come with Ubuntu Budgie, Pocillo and TelaBudgie.

To use it in Snap applications, you need to install the Snap version of the theme.

<iframe src="https://snapcraft.io/flugir-budgie-theme/embedded?button=black&screenshot=true" frameborder="0" width="100%" height="670px" style="border: 1px solid #CCC; border-radius: 2px;"></iframe>

Unfortunately, you still need to use these commands to use the theme in installed Snap applications.
And reuse them when installing new Snap applications.

``` for i in $(snap connections | grep gtk-common-themes:gtk-3-themes | awk '{print $2}'); do sudo snap connect $i flugir-budgie-theme:gtk-3-themes; done ```

``` for i in $(snap connections | grep gtk-common-themes:icon-themes | awk '{print $2}'); do sudo snap connect $i flugir-budgie-theme:icon-themes; done ```

Here are the links to the projects I used to create the Flugir theme:

Qogir theme: https://github.com/vinceliuice/Qogir-theme

GoogleDot cursors: https://github.com/ful1e5/Google_Cursor

Fluent theme: https://github.com/vinceliuice/Fluent-gtk-theme
