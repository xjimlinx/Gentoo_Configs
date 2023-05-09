### Kde-Configs

Languages    [中文](./Kde-Configs.md)

#### plasma-pa

在 KDE 中自带的管理音频的工具是 plasma-pa

```bash
sudo emerge --ask plasma-pa
# 用这条命令安装
```

另外因为部分程序打开用到了 gtk 主题，所以在编译 kde 时 USE 最好不要用 -gtk 和 -gnome,要不然在更改了自定义的主题之后如果颜色不一样会很难看

然后因为 fcitx5 在 ~amd64 keyword 里面，所以干脆直接搞最新的
在/etc/portage/make.conf 里面下两项改成这个，

```bash
ACCEPT_LICENSE="*"
# 代表接受所有协议
ACCEPT_KEYWORDS="~amd64"
# 代表像Arch那样用最新的
```
