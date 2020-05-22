<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Contents**

- [实用工具](#%E5%AE%9E%E7%94%A8%E5%B7%A5%E5%85%B7)
- [开发](#%E5%BC%80%E5%8F%91)
  - [命令行](#%E5%91%BD%E4%BB%A4%E8%A1%8C)
  - [实用工具](#%E5%AE%9E%E7%94%A8%E5%B7%A5%E5%85%B7-1)
- [音视频](#%E9%9F%B3%E8%A7%86%E9%A2%91)
- [阅读写作](#%E9%98%85%E8%AF%BB%E5%86%99%E4%BD%9C)
- [下载工具](#%E4%B8%8B%E8%BD%BD%E5%B7%A5%E5%85%B7)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

> [参考](https://github.com/jaywcjlove/awesome-mac/blob/master/README-zh.md)

# 实用工具

- [Alfred](https://www.alfredapp.com/) Mac必备效率神器
  - [个人配置](https://github.com/HelperInCa/notes/blob/master/modules/hotkey.md#alfred)
- [CheatSheet](https://www.mediaatelier.com/CheatSheet/) 按住 ⌘ 快速提醒快捷键
- [Background music](https://github.com/kyleneideck/BackgroundMusic) 独立调节各App音量, 录音
- [Keka](https://www.keka.io/) 免费文件解压
- [HandShaker](http://www.smartisan.com/apps/handshaker) Mac与安卓手机互联
  - [Itsycal](https://www.mowglii.com/itsycal/) 菜单栏上的日历	
- [Irvue](https://irvue.tumblr.com/) wallpapers from Unsplash
- [uPic](https://github.com/gee1k/uPic) 免费, 上传到图床, 支持Markdown
- [Time out](https://www.dejal.com/timeout/) 定时休息提醒
- [DBeaver](https://dbeaver.io/) SQL 客户端, 支持主流数据库(学生可免费用商业版)

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

# 音视频

- [IINA](https://github.com/iina/iina/wiki) 基于MPV的音视频播放器

  - [将chrome里的视频在IINA中打开](https://chrome.google.com/webstore/detail/open-in-iina/pdnojahnhpgmdhjdhgphgdcecehkbhfo)

    - [为何会无法打开视频](https://github.com/iina/iina/wiki/%E4%BD%BF%E7%94%A8-IINA-%E5%92%8C-youtube-dl-%E8%A7%82%E7%9C%8B%E7%BD%91%E9%A1%B5%E8%A7%86%E9%A2%91#%E4%B8%BA%E4%BD%95%E4%BC%9A%E6%97%A0%E6%B3%95%E6%89%93%E5%BC%80%E8%A7%86%E9%A2%91) 

      由于 youtube-dl 更新频繁，有时 IINA 自带的版本对于某些网站会解析失败，即提示「无法打开文件或流」

      解决: [使用你自己的 youtube-dl](https://github.com/iina/iina/wiki/%E4%BD%BF%E7%94%A8-IINA-%E5%92%8C-youtube-dl-%E8%A7%82%E7%9C%8B%E7%BD%91%E9%A1%B5%E8%A7%86%E9%A2%91#%E4%BD%BF%E7%94%A8%E4%BD%A0%E8%87%AA%E5%B7%B1%E7%9A%84-youtube-dl)

      ```shell
      # 更新youtube-dl
      $ youtube-dl -U
      ```

# 阅读写作

- [Typora](https://www.typora.io/) Markdown editor featuring seamless live preview

  - 支持ipic/upic上传到图床
  > 性能欠佳, 卡顿时暂用vs code替代
  
  

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
  100.0% (  0.5/0.5  MB) ├████████████████████████████████████████┤[1/1]   22 MB/s
    ```
  
  - Search on Google
  
    ```shell
    $ you-get "Richard Stallman eats"
    ```

 