<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Contents**

- [实用工具](#%E5%AE%9E%E7%94%A8%E5%B7%A5%E5%85%B7)
- [开发](#%E5%BC%80%E5%8F%91)
  - [命令行](#%E5%91%BD%E4%BB%A4%E8%A1%8C)
  - [实用工具](#%E5%AE%9E%E7%94%A8%E5%B7%A5%E5%85%B7-1)
  - [服务](#%E6%9C%8D%E5%8A%A1)
- [音视频](#%E9%9F%B3%E8%A7%86%E9%A2%91)
- [阅读写作](#%E9%98%85%E8%AF%BB%E5%86%99%E4%BD%9C)
- [下载工具](#%E4%B8%8B%E8%BD%BD%E5%B7%A5%E5%85%B7)
- [Chrome 插件](#chrome-%E6%8F%92%E4%BB%B6)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

> [参考](https://github.com/jaywcjlove/awesome-mac/blob/master/README-zh.md)

# 实用工具

- [Alfred](https://www.alfredapp.com/) Mac必备效率神器
  
  - [个人配置](https://github.com/HelperInCa/notes/blob/master/modules/hotkey.md#alfred)
  
- [CheatSheet](https://www.mediaatelier.com/CheatSheet/) 按住 ⌘ 快速提醒快捷键

- [Background music](https://github.com/kyleneideck/BackgroundMusic) 独立调节各App音量, 录音

- [Keka](https://www.keka.io/) 免费, 解压缩

- [HandShaker](http://www.smartisan.com/apps/handshaker) Mac与安卓手机互联
  
- [Itsycal](https://www.mowglii.com/itsycal/) 菜单栏上的日历	
  
- [Irvue](https://irvue.tumblr.com/) wallpapers from Unsplash

- [uPic](https://github.com/gee1k/uPic) 免费, 上传到图床, 支持Markdown

- ~~[Time out](https://www.dejal.com/timeout/) 定时休息提醒~~

  [stretchly](https://github.com/hovancik/stretchly) 开源免费

- [DBeaver](https://dbeaver.io/) SQL 客户端, 支持主流数据库(学生可免费用商业版)

- [1password](https://1password.com/zh-cn/) 密码管理器, from one password to "1password"!

# 开发

## 命令行

> [参考](https://github.com/herrbischoff/awesome-macos-command-line#readme)

- [Zsh](https://www.zsh.org/) shell

  - [个人配置](https://github.com/HelperInCa/notes/blob/master/DevDocs.md#zsh)

- [trash](https://github.com/ali-rantakari/trash) allow `rm` to move files to .Trash/ and have the "put back" feature

- [doctoc](https://github.com/thlorenz/doctoc) Generates table of contents for markdown files inside local git repository.

  ```bash
  doctoc /path/to/file [...]
  ```

  - generate links compatible with other sites

    ```shell
    --bitbucket bitbucket.org
    --nodejs    nodejs.org
    --github    github.com
    --gitlab    gitlab.com
    --ghost     ghost.org
    ```

  - Use the `--maxlevel` option to limit TOC entries to headings only up to the specified level; e.g., `doctoc --maxlevel 3`

## 实用工具

- [Dash](https://kapeli.com/dash) API 离线文档
- [iTerm2](http://www.iterm2.com/) 替代Terminal

## 服务

- [jsDelivr](https://www.jsdelivr.com/) 免费公共CDN, 可加速npm, GitHub, WordPress

# 音视频

- [IINA](https://github.com/iina/iina/wiki) 基于MPV的音视频播放器

  - [将chrome里的视频在IINA中打开](https://chrome.google.com/webstore/detail/open-in-iina/pdnojahnhpgmdhjdhgphgdcecehkbhfo)

    - [为何会无法打开视频](https://github.com/iina/iina/wiki/%E4%BD%BF%E7%94%A8-IINA-%E5%92%8C-youtube-dl-%E8%A7%82%E7%9C%8B%E7%BD%91%E9%A1%B5%E8%A7%86%E9%A2%91#%E4%B8%BA%E4%BD%95%E4%BC%9A%E6%97%A0%E6%B3%95%E6%89%93%E5%BC%80%E8%A7%86%E9%A2%91) 

      由于 youtube-dl 更新频繁，有时 IINA 自带的版本对于某些网站会解析失败，即提示「无法打开文件或流」

      解决: [使用你自己的 youtube-dl](https://github.com/iina/iina/wiki/%E4%BD%BF%E7%94%A8-IINA-%E5%92%8C-youtube-dl-%E8%A7%82%E7%9C%8B%E7%BD%91%E9%A1%B5%E8%A7%86%E9%A2%91#%E4%BD%BF%E7%94%A8%E4%BD%A0%E8%87%AA%E5%B7%B1%E7%9A%84-youtube-dl)

      ```shell
      # 更新youtube-dl
      $ sudo youtube-dl -U
      ```

# 阅读写作

- [Typora](https://www.typora.io/) Markdown editor featuring seamless live preview

  - 支持ipic/upic上传到图床
  > 性能欠佳

- [语雀](https://www.yuque.com/) 阿里的云端知识库(很多功能. 目前我只是用来写Markdown文档, 可以写专栏)
  
- [Stickies](https://support.apple.com/zh-cn/guide/stickies/welcome/mac) MacOS便签
  
  

# 下载工具

- [youtube-dl](https://github.com/ytdl-org/youtube-dl) download videos from YouTube and a few [more sites](http://ytdl-org.github.io/youtube-dl/supportedsites.html)

  ```shell
  $ youtube-dl https://www.youtube.com/watch?v=jNQXAC9IVRw
  ```

  - configuration `~/.config/youtube-dl/config`

    
  
- [you-get](https://github.com/soimort/you-get) download media contents from web

  ```shell
  $ you-get 'https://www.youtube.com/watch?v=jNQXAC9IVRw'
  ```

  - before downloading, use `-i` to see all the quality and formats 

  - Use the `-o` to set the path, and `-O` to set the name 
  
  - `you-get` will scrape the web page and try to figure out if there's anything interesting to you
  
    ```shell
    $ you-get http://kopasas.tumblr.com/post/69361932517
    Site:       Tumblr.com
    Title:      kopasas
    Type:       Unknown type (None)
    Size:       0.51 MiB (536583 Bytes)
    
    Site:       Tumblr.com
    Title:      tumblr_mxhg13jx4n1sftq6do1_1280
    Type:       Portable Network Graphics (image/png)
    Size:       0.51 MiB (536583 Bytes)
  
    Downloading tumblr_mxhg13jx4n1sftq6do1_1280.png ...
    100.0%(0.5/0.5MB)├████████████████████████████████████████┤[1/1]22MB/s   
    ```
  
  - Search on Google
  
    ```shell
    $ you-get "Richard Stallman eats"
    ```

 

# Chrome 插件

- [Vimium](https://chrome.google.com/webstore/detail/vimium/dbepggeogbaibhgnhhndojpepiihcmeb) 使用Vim快捷键操作Chrome, 告别鼠标!

- [沙拉查词](https://chrome.google.com/webstore/detail/%E6%B2%99%E6%8B%89%E6%9F%A5%E8%AF%8D-%E8%81%9A%E5%90%88%E8%AF%8D%E5%85%B8%E5%88%92%E8%AF%8D%E7%BF%BB%E8%AF%91/cdonnmffkdaoajfknoeeecmchibpmkmg?hl=zh-CN) 划词翻译

- [Adblock](https://www.getadblock.com/) 

  > 部分网站要求关了Adblock才能打开

- [Grammarly](https://chrome.google.com/webstore/detail/grammarly-for-chrome/kbfnbcaeplbcioakkpcpgfkobkghlhen) 检查语法

- [JSON Formatter](https://chrome.google.com/webstore/detail/json-formatter/bcjindcccaagfpapjjmafapmmgkkhgoa?hl=zh-CN) Make JSON easy to read

- [OneTab](https://chrome.google.com/webstore/detail/onetab/chphlpgkkbolifaimnlloiipkdnihall?hl=zh-CN) 将所有标签页转换成一个列表。当您需要再次访问这些标签页时，可以单独或全部恢复它们。

- [Octotree](https://chrome.google.com/webstore/detail/octotree/bkhaagjahfmjljalopjnoealnfndnagc?hl=zh-CN) 让GitHub项目以树状显示

- [Magic Enhancer For YouTube](https://autohdforyoutube.com/) Auto HD, Video Ad Blocking, Cinema Mode and More

- [Proxy SwitchyOmega](https://chrome.google.com/webstore/detail/proxy-switchyomega/padekgcemlokbadohgkifijomclgjgif?hl=zh-CN) 管理和切换多个代理设置

  > [GFWList](https://raw.githubusercontent.com/gfwlist/gfwlist/master/gfwlist.txt) 

- [h264ify](https://chrome.google.com/webstore/detail/h264ify/aleakchihdccplidncghkekgioiakgal) 将VP8/9 改成H.264解码(不能VP9硬解, cpu占用高!)

  缺点: 无法看1080p以上的视频

- [Checker Plus for Gmail](https://chrome.google.com/webstore/detail/checker-plus-for-gmail/oeopbcgkkoapgobdbedcemjljbihmemj?hl=zh-CN) 不用打开Gmail就能管理, 支持多账户

- [Gmail Sender Icons](https://chrome.google.com/webstore/detail/gmail-sender-icons/jniljaamodclkmphgkgkooplflhkadpg) 显示邮件发送者域名和logo

- [Simple Gmail Notes](https://chrome.google.com/webstore/detail/simple-gmail-notes/jfjkcbkgjohminidbpendlodpfacgmlm) 给邮件添加备注, 存在自己的Google Drive

