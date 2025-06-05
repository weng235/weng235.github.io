---
title: Cloudflare(一)
description: Cloudflare绑定域名和托管以及DNS记录的使用
date: 2025-06-05 9:00:00 +0800
categories: [技术,Cloudflare]
tags: [Technology]
---

## 🚀 完成绑定和托管

> 没有Cloudflare账号的先完成注册（过于简单不做说明）

### 📝 步骤一：添加域名
1. 进入账户主页点击 **"添加域"**

![主页界面说明](/assets/imgs/20250605/01.png){: width="972" height="589" }

2. 输入已经注册域名并且 **确认可用** 后点击继续

![绑定域名界面说明](/assets/imgs/20250605/02.png){: width="972" height="589" }

3. 选择你的计划（💡 提示：免费套餐够用）

### 📝 步骤二：配置名称服务器
1. 找到分配给你的两个名称服务器地址

![名称服务器界面说明](/assets/imgs/20250605/03.png){: width="972" height="589" }

2. 复制到你的DNS提供商（这里我用的DigitalPlat，也可以是腾讯阿里的，根据自己情况来）

![DNS提供商界面说明](/assets/imgs/20250605/04.png){: width="972" height="589" }

3. 看到以下界面即为成功

![成功界面说明](/assets/imgs/20250605/05.png){: width="972" height="589" }

> ⏳ a few moments later...

✨ Cloudflare和DigitalPlat都会给你发送成功的邮件，代表你完成了绑定和托管

## 🔧 DNS记录的使用

这里我使用我部署的中转gemini api作为例子，你可以选择：
- 📦 绑定git来拉取代码
- 💻 从本地上传

![pages界面说明](/assets/imgs/20250605/06.png){: width="972" height="589" }

### 📝 配置步骤
1. 点击添加自定义域名，拿到cname值（💡 提示：pages需要自己配置DNS，worker会自动设置）

2. 如下图添加cname记录，然后就可以访问到你域名下的网站了

![DNS记录界面说明](/assets/imgs/20250605/07.png){: width="972" height="589" }
