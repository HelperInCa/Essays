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

  1. 查这些域名的IP并测速: `github.com` `github.global.ssl.fastly.net`
  `assets-cdn.github.com`
  2. `sudo vi /etc/hosts`
  
  
  


