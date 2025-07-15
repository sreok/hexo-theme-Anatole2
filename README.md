## 介绍

<div align=center>
<img src="https://raw.githubusercontent.com/sreok/hexo-theme-Anatole2/refs/heads/main/source/images/logo.png" width = "200" height = "200" alt="Anatole2" />
</div>

基于Core的Anatole主题进行修改，[项目地址](https://github.com/mrcore/hexo-theme-Anatole-Core)

[Ben02原主题地址](https://github.com/Ben02/hexo-theme-Anatole) - [主题使用文档](https://github.com/Ben02/hexo-theme-Anatole/wiki)

预览：https://sreok.cn

<div align=center>
<img src="https://raw.githubusercontent.com/sreok/sreok.github.io/refs/heads/master/images/c3d82da8df320cc6fdf6654ba5a7984b.png" alt="Anatole2" />

<img src="https://raw.githubusercontent.com/sreok/sreok.github.io/refs/heads/master/images/0ae96558f2247fef8963572c1cab3cd4.png" alt="Anatole2" />
</div>

## 使用

1. 进入hexo的blog目录
```
git clone https://github.com/sreok/hexo-theme-Anatole2.git
```

2. 应用主题
修改根目录`_config.yml`文件
```
theme: anatole2
```

3. 修改主题信息
修改`themes/Anatole2/_config.yml`文件
```
# 关键字
keywords: Elijah博客,Elijah Blog,博客,Elijah,Linux,Kubernetes,Docker,DevOps
# 作者
author: Elijah
# 网站左侧描述
description: 描述信息
# 如需修改icon,请替换 source/images/favicon.ico 文件
avatar: /images/favicon.png
beian: 冀ICP备xxxxxxxxxx号
# 版权
copyright: 2020 - 2025


# 社交账号
github: https://github.com/sreok
mail: mailto:admin@vsoul.cn
zhihu: 
qq: 
wechat: 
rss: true
```

4. 生成tags页面（可选）

开启tags页面
```
hexo new page tags
```
修改根目录`source/tags/index.md`
```
---
title: 标签
type: "tags"
---
```

5. 开启留言板（可选）
修改`themes/Anatole2/_config.yml`
```
# Valine 评论，如何配置请看官网 https://valine.js.org
valine:
  enable: true # if you want use valine, please set enable: true
  appid: xxxxxxxxxxxxxxxxxxxxxxxxxxxx
  appkey: xxxxxxxxxxxxxxxxxxxxxxxx
  notify: true # true/false:mail notify !!!Test,Caution. https://github.com/xCss/Valine/wiki/Valine-%E8%AF%84%E8%AE%BA%E7%B3%BB%E7%BB%9F%E4%B8%AD%E7%9A%84%E9%82%AE%E4%BB%B6%E6%8F%90%E9%86%92%E8%AE%BE%E7%BD%AE
  verify: false # true/false:verify code
  avatar: 'hide' # avatar style https://github.com/xCss/Valine/wiki/avatar-setting-for-valine
  placeholder: 念念不忘，必有回响... # comment box placeholder
  serverURLs: 
```

新建留言板页面
```
hexo new page guestbook
```

修改根目录`source/guestbook/index.md`（DEMO）
此页可不修改为空即可
```
---
title: 留言板
date: 2025-05-26 15:06:03
type: "guestbook"
---
<div align="center">
  
  <!-- dynamic typing effect 文本 -->
  <img src="https://capsule-render.vercel.app/api?type=blur&height=300&color=gradient&text=留言板&fontColor=888fff&section=footer&reversal=true&fontAlign=50&fontSize=55&textBg=false" />

</div>
```
注：其他页面关闭评论功能（例如关于页面），在页面开头处`---`内添加`comments: false`。
```
---
title: 标题
date: 
auther: 作者
categories:
 - 分类
tags: 
 - 标签
comments: false # 添加此行关闭评论
---
```

6. 开启本地搜索（可选）

修改`themes/Anatole2/_config.yml`文件
```
local_search: true
```

7. 开启友链页面（可选）

新建页面
```
hexo new page links
```

博客根目录`source`下新建`index.md`,输入以下内容保存。
```
---
title: 友链
layout: links
---
```

博客根目录`source`下创建`_data`目录，并新建`links.yml`
以下是友链格式
```
- title: GitHub
  url: https://github.com/
  avatar: https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png
  description: 全球最大同性交友网站
- title: Hexo
  url: https://hexo.io/
  avatar: https://hexo.io/logo.svg
  description: 快速、简洁且高效的博客框架
```

8. 生成并使用
```
hexo generate
hexo server
```

9. 部署到Github Page

[文档](http://localhost:4000/2025/05/27/%E3%80%90%E7%AC%94%E8%AE%B0%E3%80%91%E5%9F%BA%E4%BA%8Egithub%20page%E5%88%9B%E5%BB%BAhexo%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2/)
```
hexo deploy
```

## 声明
本主题仅用于学习，非前端工作者，修改部分仅满足个人使用习惯。

如有修改建议可联系邮箱: [lihaoxuan@vsoul.cn](mailto:someone@example.com)

## 更新内容

2025.7.15 更新
1. 新增底部分页显示
2. 取消左侧栏中全大写标题


2025.7.2 更新

1. 新增友链页面`layout: links`

2025.7.1 更新

1. 新增本地搜索功能
2. 修复移动端导航超出换行显示问题

2025.5.29 修改部分内容

1. 圆形头像
2. 右上角图标可通过`_config.yml`修改`right_top_logo: true`
3. 页面比例调整25%-75%，让阅读更方便

2025.5.27  首次提交

1. 新增rss订阅功能
2. 新增社交微信图标（链接跳转需手动指定，官方暂不支持链接跳转添加好友）
3. 优化底部信息
4. 新增友链功能
