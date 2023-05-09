### 字体设置

语言 [English](./Fonts.md)

> 因为在 kde 界面中有些程序打开后字体和 kde 设置里面字体设置的不一样，好像是更底层的设置，根据 Gentoo 官方的 Wiki，需要在以下的地方进行操作

#### [Gentoo Wiki Fontconfig](https://wiki.gentoo.org/wiki/Fontconfig/zh-cn)

```bash
sudo eselect fontconfig enable 51-local.conf
# 启用51-local.conf配置文件
```

```bash
sudo vim /etc/fonts/local.conf
# 自定义想要的字体
```

在/etc/fonts/local.conf 这个文件里面输入你想要的字体
然后在终端里面输入如下命令：

```bash
sudo xset fp rehash
```

然后重启应用，你就会发现字体变成了你设置的。
