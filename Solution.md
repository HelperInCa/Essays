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
    sudo softwareupdate --ignore "macOS Big Sur"
    defaults write com.apple.systempreferences AttentionPrefBundleIDs 0 && killall Dock 
    ```
    
- Another app is currently holding the yum lock

    yum在锁定状态中。
    可以通过强制关掉yum进程：`rm -f /var/run/yum.pid`

- 环境变量

    `vi /etc/profile`

    `export PATH=$PAHT:<PATH 1>:<PATH 2>:<PATH 3>:--------:< PATH n >`

    `source /etc/profile`
    
- 清理 Mac 微信缓存

    ```sh
    rm -f /Users/${用户名}/Library/Containers/com.tencent.xinWeChat/Data/Library/Application Support/com.tencent.xinWeChat/2.0b4.0.9/${一串英文数字}/Message/MessageTemp/*
    ```

    

- ssh登录失败

    报错: `no matching host key type found. Their offer: ssh-dss`

    解决方法: `ssh -oHostKeyAlgorithms=+ssh-dss <username>@<ip>`

- 关闭 Chrome 更新

    *建议备份*

    > 保存在~/Downloads/

    1. 关闭 Chrome

    2. ```shell
        sudo rm -rf /Library/Google/GoogleSoftwareUpdate/GoogleSoftwareUpdate.bundle
        ```

    3. 打开Chrome,点击`帮助`->`关于`,查看是否无法更新

        
    
- homebrew 换国内源(包括复原)

    [1](https://mirrors.tuna.tsinghua.edu.cn/help/homebrew/)

- vim 粘贴时格式混乱

    [缩进导致](https://blog.51cto.com/u_15060513/4627037)

    ```shell
    #进入普通模式
    :set paste
    #粘贴
    :set nopaste
    ```

    

- ERR_PROXY_CONNECTION_FAILED

    [参考](https://zhuanlan.zhihu.com/p/406660822)

    - 刷新dns缓存

    ```shell
    sudo killall -HUP mDNSResponder
    sudo dscacheutil -flushcache
    ```

    
