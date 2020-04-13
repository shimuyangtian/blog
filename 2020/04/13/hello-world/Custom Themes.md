## Nginx简介

NGINX是一个免费、开源、高性能、轻量级的HTTP和反向代理服务器，也是一个电子邮件（IMAP/POP3）代理服务器，其特点是占有内存少，并发能力强。 Nginx 因为它的稳定性、丰富的模块库、灵活的配置和较低的资源消耗而闻名 。

Nginx由内核和一系列模块组成，内核提供web服务的基本功能，如启用网络协议，创建运行环境，接收和分配客户端请求，处理模块之间的交互。Nginx的各种功能和操作都由模块来实现。Nginx的模块从结构上分为核心模块、基础模块和第三方模块。



核心模块： HTTP模块、EVENT模块和MAIL模块



基础模块： HTTP Access模块、HTTP FastCGI模块、HTTP Proxy模块和HTTP Rewrite模块



第三方模块： HTTP Upstream Request Hash模块、Notice模块和HTTP Access Key模块及用户自己开发的模块

## Get Typora Themes

We have an office website [Typora Theme Gallery](http://theme.typora.io) for designers/developers to share their custom themes with others. You could download theme from there.

## Install Custom Themes

1. Open Theme Folder. (see instructions below)
2. Copy or move `.css` file and related resources, like fonts or images, into the newly opened folder.
3. Restart typora, then select it from `Themes` menu.

## Open Theme Folder

### macOS

Open preference panel by <code>cmd+`</code>, then click "Open Theme Folder"

<img src="img/Snip20160921_1.png" style="zoom:50%" />

### Windows/Linux

Open preference panel from `File` → `Preference` from menubar, then click "Open Theme Folder":

<img src="img/Snip20160921_2.png" style="zoom:50%" />

## Modify Current Styles

Sometimes, you may just want to change font family for all themes, for change font-color for headings for a specific themes. In this case, you do not need to copy/modify a whole exiting css file, just [Add Custom CSS](https://support.typora.io/Add-Custom-CSS/) is enough. In brief:

- Create & write a `base.user.css` under theme folder, the css rules inside it will be applied to all themes.
- Create & write a `{theme-css-name}.user.css` under theme folder, the css rules inside it will only be applied to theme file `{theme-css-name}.css`.

Please note that the built-in CSS theme files will get overwritten completely on typora version up, so, write your custom css into `*.user.css`, instead of the existing files, will prevent your modifications from being lost after update.

## Write My Own Theme

Please refer to [Write Custom Theme for Typora](http://theme.typora.io/doc/Write-Custom-Theme/).