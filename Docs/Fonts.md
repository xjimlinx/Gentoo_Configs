### Font Configs

Languages    [中文](./Fonts-zh.md)

> 因为在 kde 界面中有些程序打开后字体和 kde 设置里面字体设置的不一样，好像是更底层的设置，根据 Gentoo 官方的 Wiki，需要在以下的地方进行操作

#### [Gentoo Wiki Fontconfig](https://wiki.gentoo.org/wiki/Fontconfig/zh-cn)

```bash
sudo eselect fontconfig enable 51-local.conf
```

```bash
sudo vim /etc/fonts/local.conf
```

Input your favorite Fonts into this file: /etc/fonts/local.conf
Then input this command on terminal:

```bash
sudo xset fp rehash
```

Then reopen the application, you will find out that the fonts of the app has been changed.
