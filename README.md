# Actions-OpenWrt
**由于上游包冲突过多及编译环境不稳定等原因，现已停止维护😕**

**最新发布仅包含下列部分插件，且需要手动更改默认IP及主题**

- 使用Action云编译自用的OpenWrt.
- 原作者仓库：https://github.com/P3TERX/Actions-OpenWrt

## 定制内容

### 类型
System Target --> x86 \
Subtarget --> x86_64 \
Target Profile --> Generic x86/64 

### 镜像格式保持默认即可（squashfs，ext4）
Target Images -->

### 调整分区大小
Target Images --> Kernel partition size --> 256 \
Target Images --> Root filesystem partition size --> 1024 

### 开启 IPv6
Network --> odhcp6c \
Network --> odhcpd-ipv6only \
LuCI --> Protocols --> luci-proto-ipv6 \
LuCI --> Protocols --> luci-proto-ppp \
NetWork --> Firewall --> ip6tables-extra \
NetWork --> Firewall --> ip6tables-mod-nat

### 开启适用于 VMware 的 VMware Tools
Utilities --> open-vm-tools \
Utilities --> open-vm-tools-fuse 

### LuCI
LuCI --> Collections --> luci

### 插件
| LuCI --> Applications -->  |
| --- |
| luci-app-advanced |
| luci-app-advanced-reboot |
| luci-app-aliyundrive-webdav |
| luci-app-aria2 |
| luci-app-bypass |
| luci-app-ddns |
| luci-app-ddns-go |
| luci-app-emby |
| luci-app-istorepanel |
| luci-app-istorex |
| luci-app-jellyfin |
| luci-app-openclash |
| luci-app-qbittorrent |
| luci-app-samba4 |

### 主题
luci-theme-argon \
luci-theme-argone \
luci-theme-design

### 语言
LuCI --> Modules --> Translations --> Chinese Simplified (zh_Hans) \
LuCI --> Modules --> Translations --> Chinese Traditional (zh_Hant)

## License

[MIT](https://github.com/Yppup/OpenWrt_x86_64_firmware/blob/dev/LICENSE) © [**P3TERX**](https://p3terx.com)
