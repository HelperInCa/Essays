<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Contents**

- [待解决](#%E5%BE%85%E8%A7%A3%E5%86%B3)
- [已解决](#%E5%B7%B2%E8%A7%A3%E5%86%B3)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# 待解决

# 已解决

- GitHub CDN 被DNS污染

  修改hosts, 绕过国内dns解析:

  1. `ping`这些域名的IP并测速: `github.com` `github.global.ssl.fastly.net`
      `assets-cdn.github.com`

  2. `sudo vi /etc/hosts`

  3. 刷新DNS缓存

     `sudo killall -HUP mDNSResponder`

- 手动切换集/独显

  ```shell
  sudo pmset -a GPUSwitch 0
  ```
  
  > 0, 强制使用核显，
  >
  > 1, 强制使用独显，
  >
  > 2, 自动切换图形卡
  
  

- 计划中的时间节点要落实, 及时沟通进展(不管进度如何)

    每件事都有时间效应的, 及时暴露风险

- ~~关闭 Mac 系统更新~~

    ```shell
    sudo softwareupdate --ignore "macOS Catalina"
    defaults write com.apple.systempreferences AttentionPrefBundleIDs 0 && killall Dock 
    ```
    


