不稳定，经常断网，然后重启，时不时5G wifi 丢失

iptables -I FORWARD -p tcp -m connlimit -connlimit-above 100 -j REJECT

iptables -I FORWARD -p udp -m connlimit -connlimit-above 41 -j REJECT


Changes:

.config

remove all features, add ssr-plus


https://github.com/gcp70908/PSG1218/blob/master/.github/workflows/build-openwrt-lean.yml

REPO_URL: https://github.com/gcp70908/lede

on:
  repository_dispatch:
  workflow_dispatch:
    inputs:
      ssh:
        description: 'SSH connection to Actions'
        required: false
        default: 'false'



# OpenWrt firmware for K2-PSG1218-A
固件采用GitHub Actions不定时自动云编译斐讯K2-PSG1218-A。  
Auto build OpenWrt firmware for K2-PSG1218-A via GitHub Actions

# 致谢大佬&Thanks

https://github.com/coolsnowwolf/lede

https://github.com/P3TERX/Actions-OpenWrt/

https://github.com/Lienol/openwrt-package

.....



# 最新版下载&Download Latest
[![GitHub release (latest by date)](https://img.shields.io/github/v/release/leopardciaw/PSG1218?style=for-the-badge&label=Download)](https://github.com/leopardciaw/PSG1218/releases/latest)


[所有已发布 & All Release](https://github.com/leopardciaw/PSG1218/releases)

# 请注意
1.集成的插件只是自己需要用到的，请多多包涵。  
2.源码来自https://github.com/coolsnowwolf/lede，
除了增减插件和主题、修改管理IP外，未做其他修改，有问题请直接到
https://github.com/coolsnowwolf/lede/issues 这里提交issue，提交issues请注意基本的礼仪和格式，翻看之前是否有大佬已提出相关issue。  
3.才疏学浅、时间有限，回答不了任何技术问题哈，只是定时或不定时更新下大雕的源码编译。
