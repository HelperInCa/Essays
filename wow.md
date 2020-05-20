<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Contents**

- [好用的工具](#%E5%A5%BD%E7%94%A8%E7%9A%84%E5%B7%A5%E5%85%B7)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# 好用的工具

- [you-get](https://github.com/soimort/you-get) download media contents from web

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