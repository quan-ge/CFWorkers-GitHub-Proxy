# CF-Workers-GitHub-Proxy
#### 本仓库为优化改版

> [!WARNING]
> 项目可能会触发**疑似钓鱼网站**警告或域名封禁，
> 
> 请通过环境变量 `URL` 赋值 **nginx** 或 `URL302` 设置302跳转域名进行伪装。
>
> 请一定要禁用默认的'workers.dev'域名

> [!WARNING]
> 根据 [Cloudflare 协议](https://www.cloudflare.com/zh-cn/terms/) 中，2.2.1 第 (j) use the Services to provide a virtual private network or other similar proxy services.
>
> 使用本服务可能存在被 Cloudflare 封号的潜在风险，请自行斟酌使用风险。
>
> 如果你选择了“根据主机名选择对应的上游地址”方式部署，你**可能**会:
> 
> 被 Netcraft 扫描到，收到警告邮件
>
> 被 Netcraft 同步到 Google Safe Browsing 标记为钓鱼网站
>
> 被 Netcraft 投诉到 Cloudflare 标记为钓鱼网站, 无法正常 pull 镜像
>
> 收到律师函

## 服务预览
<details>
  <summary>桌面端预览</summary>
  <img src="src/desktop.png" alt="desktop" />
</details>
<details>
  <summary>移动端预览</summary>
  <img src="src/mobile.png" alt="mobile" />
</details>

## 简介
GitHub Release、Archive以及项目文件的加速项目，支持clone，GitHubAPI，使用 Cloudflare Workers/Pages 部署

## 公共DEMO

 - `https://ghfile.geekertao.top/`
 - `https://gh.geekertao.top/`
 - `https://github.dpik.top/`
 - `https://gh.felicity.ac.cn/`
 - `https://fgp.120322.dpdns.org/`

***大量使用建议自行部署，以上域名仅为演示使用，可以轻量使用。***

## 使用

直接在copy出来的url前加网址即可

也可以直接访问，在input输入

---

访问私有仓库可以通过 [#71](https://github.com/hunshcn/gh-proxy/issues/71)

在域名前`user:TOKEN@`的方法

例如`git clone https://user:TOKEN@ghfile.XXXX.top/https://github.com/xxxx/xxxx`

---

以下都是合法输入（仅示例，文件不存在）：

- 分支源码：https://github.com/hunshcn/project/archive/master.zip

- release源码：https://github.com/hunshcn/project/archive/v0.1.0.tar.gz

- release文件：https://github.com/hunshcn/project/releases/download/v0.1.0/example.zip

- 分支文件：https://github.com/hunshcn/project/blob/master/filename

- commit文件：https://github.com/hunshcn/project/blob/1111111111111111111111111111/filename

- gist：https://gist.githubusercontent.com/cielpy/351557e6e465c12986419ac5a4dd2568/raw/cmd.py

- api：https://api.github.com/repos/Geekertao/CF-Workers-GitHub-Proxy



## Workers 部署方法
### 部署 Cloudflare Worker：

   - 在 Cloudflare Worker 控制台中创建一个新的 Worker。
   - 将 [workers.js](/worker.js)  的内容粘贴到 Worker 编辑器中。

## Pages 部署方法
### 部署 Cloudflare Pages：

   - Fork本项目。
   - 在 Cloudflare Worker 控制台中创建一个新的 Worker。
   - 链接你Fork的仓库。


# 致谢
[gh-proxy](https://github.com/hunshcn/gh-proxy)、[jsproxy](https://github.com/EtherDream/jsproxy/)、[cmliu/CF-Workers-GitHub](https://github.com/cmliu/CF-Workers-GitHub/)、[hubporg/CF-GitHub-Proxy](https://github.com/hubporg/CF-GitHub-Proxy)

# 赞助
<a href="https://afdian.com/a/QUAN_GE" target="_blank" rel="noopener noreferrer" style="flex-shrink: 0;">
      <img src="https://img.shields.io/badge/💵_爱发电-FF4D4D?style=flat-square&logo=usd&logoColor=white" alt="爱发电" style="max-height: 50px;">
    </a>


