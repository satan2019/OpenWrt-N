# Actions-OpenWrt

**更新日志**
- 20231015 更新内核版本 6.1.57，集成 `PassWall`

说明：
- 本项目使用 Github Actions 下载 [Lean](https://github.com/coolsnowwolf/lede) 的 `Openwrt` 源码仓库，进行云编译。
- 本项目使用定时编译（北京时间每日0点开始自动运行编译）。
- 本项目编译固件适配斐讯 `Phicomm-N1` 盒子，如需刷机，可直接下载 [releases](https://github.com/kaikai8191/OpenWrt-N1/releases/latest) 内固件。
- 本项目相对源码默认设置做了如下更改：

**增强项**：（**打勾项**默认**编译**入固件；**未打勾项**默认**不编译**入固件。）
  - [x] 编译 `PassWall`
  - [x] 添加主题 `argon` 并设置为默认
  - [x] 添加第三方插件 `luci-app-adguardhome`
  - [x] 添加第三方插件 `luci-app-amlogic`
  - [x] 添加第三方插件 `luci-app-vssr`
  - [x] 添加第三方插件 `luci-app-openclash`

**精简项**：
  - [x] luci-app-accesscontrol
  - [x] luci-app-ddns
  - [x] luci-app-rclone
  - [x] luci-app-upnp
  - [x] luci-app-vsftpd

## 感谢 ❤️
- 源码来源： [Lean](https://github.com/coolsnowwolf/lede) 的 Openwrt 源码仓库
- 脚本来源： [P3TERX](https://github.com/P3TERX/Actions-OpenWrt) 的 使用 GitHub Actions 云编译 OpenWrt
- 打包脚本： [Flippy](https://github.com/ophub/flippy-openwrt-actions) 的 OpenWrt 打包脚本 Actions
