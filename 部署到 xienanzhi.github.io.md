# 把网站放到 xienanzhi.github.io

目录里只有 `index.html` 一个文件，它就是完整网站，不需要别的。

> **先确认一件事**：`xienanzhi.github.io` 这个网址能不能用，取决于你的 GitHub 用户名是不是正好叫 `xienanzhi`。
> 打开 https://github.com/xienanzhi 看一眼：
> - 能打开 → 就是你的账号，继续下面步骤。
> - 打不开（404）→ 说明用户名不是这个，去 GitHub → Settings → Account → **Change username** 改成 `xienanzhi`，改完再来；不想改用户名的话，仓库名就得用你的真实用户名。
>
> 你电脑 git 里配的名字是 `202301020131xieyongsheng`，那是本地提交署名，跟 GitHub 用户名不是一回事，别搞混。

## 一、建仓库（仓库名必须严格）

1. 登录 GitHub，右上角 `+` → **New repository**
2. Repository name 填：**`xienanzhi.github.io`**（一字不差）
3. 选 **Public**，勾选 **Add a README file**
4. 点 **Create repository**

> 仓库名写错，网站就打不开。

## 二、上传 index.html

1. 进入刚建好的仓库，点 **Add file** → **Upload files**
2. 把 `index.html` 拖进上传框
3. 拉到底部，点绿色 **Commit changes**

> 文件名必须是 `index.html`，改一个字母访问就是 404。

## 三、开启 Pages

1. 仓库顶部点 **Settings**
2. 左侧菜单找 **Pages**
3. Build and deployment：
   - Source 选 **Deploy from a branch**
   - Branch 选 **main**，文件夹选 **/ (root)**
4. 点 **Save**

## 四、访问

等 1~5 分钟（太早访问会 404），打开：

```
https://xienanzhi.github.io
```

## 常见问题

| 现象 | 原因 |
| --- | --- |
| 404 | 仓库名或用户名不对 / 没有 index.html / 保存后等待时间不够 |
| 乱码 | html 头部必须有 `<meta charset="UTF-8">`（本文件已有） |
| 图片不显示 | 路径写错（本游戏不使用外部图片，全部 Canvas 绘制） |

## 国内访问慢

GitHub 服务器在海外，长沙这边打开有时会卡。开着瓦特工具箱的 GitHub 加速会顺畅很多。
嫌麻烦的话，直接用已经部署好的在线地址就行，不用自己传 GitHub。

## 更新网站

改完 `index.html` 重新上传并提交，等几分钟网页会自动更新。
