## 介绍

<div align=center>
<img src="https://raw.githubusercontent.com/sreok/hexo-theme-Anatole2/refs/heads/main/source/images/logo.png" width = "200" height = "200" alt="Anatole2" />
</div>

基于Core的Anatole主题进行修改，项目地址：https://github.com/mrcore/hexo-theme-Anatole-Core

Ben02原主题地址：https://github.com/Ben02/hexo-theme-Anatole

主题使用文档：https://github.com/Ben02/hexo-theme-Anatole/wiki

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

2. 修改根目录`_config.yml`文件
```
theme: anatole2
```

3. 修改`themes/Anatole2/_config.yml`文件
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

4. 生成tags页面、留言板页面（可选）
开启tags页面
```
hexo new page tags
```
修改根目录`source/tags/index.md`
```
---
title: tags
date: 2025-05-26 15:04:08
type: "tags" # 添加此行
---
```

开启留言板（需打开Valine 评论，详见_config.yml）
```
hexo new page guestbook
```

修改根目录`source/guestbook/index.md`（DEMO）
此页可不修改为空即可
```
---
title: 
date: 2025-05-26 15:06:03
type: "guestbook"
---
<div align="center">
  
  <!-- dynamic typing effect 文本 -->
  <img src="https://capsule-render.vercel.app/api?type=blur&height=300&color=gradient&text=留言板&fontColor=888fff&section=footer&reversal=true&fontAlign=50&fontSize=55&textBg=false" />

</div>
```
注：其他页面关闭评论功能（例如关于页面），在页面开头处`---`内添加`comments: false`。


5. 生成并使用
```
hexo generate
hexo server
```

## 声明
本主题仅用于学习，非前端工作者，修改部分仅满足个人使用习惯。

如有修改建议可邮箱联系

## 更新内容

2025.5.29 修改部分内容

1. 圆形头像
2. 右上角图标可通过`_config.yml`修改`right_top_logo: true`
3. 页面比例调整25%-75%，让阅读更方便

2025.5.27  首次提交

1. 新增rss订阅功能
2. 新增社交微信图标（链接跳转需手动指定，官方暂不支持链接跳转添加好友）
3. 优化底部信息
4. 新增友链功能
