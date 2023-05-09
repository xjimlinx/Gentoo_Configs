sudo eselect fontconfig enable 51-local.conf
sudo vim /etc/fonts/local.conf
Input your favorite Fonts into this file: /etc/fonts/local.conf
Then input this command on shell:
sudo xset fp rehash
Then reopen the application, you will find out that the fonts of the app has been changed.
