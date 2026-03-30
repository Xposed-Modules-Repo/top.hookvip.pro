<div align="center">
<h1>NewHookVip</h1>

<a href="https://github.com/Xposed-Modules-Repo/top.hookvip.pro/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/Xposed-Modules-Repo/top.hookvip.pro?label=Stars"></a>
<a href="https://github.com/Xposed-Modules-Repo/top.hookvip.pro/releases"><img alt="GitHub all releases" src="https://img.shields.io/github/downloads/Xposed-Modules-Repo/top.hookvip.pro/total?label=Downloads"></a>
<a href="https://github.com/Xposed-Modules-Repo/top.hookvip.pro/releases/latest"><img alt="GitHub latest release" src="https://img.shields.io/github/v/release/Xposed-Modules-Repo/top.hookvip.pro"></a>

<a href="https://t.me/HookVipCl"><img alt="Telegram Channel" src="https://img.shields.io/badge/Telegram-频道-blue.svg?logo=telegram"></a>
<a href="https://t.me/HookVipChat"><img alt="Telegram Group" src="https://img.shields.io/badge/Telegram-群组-blue.svg?logo=telegram"></a>

<p>用于解锁部分 App 会员功能、部分高级功能，解除部分功能限制，并提供拓展功能的 Xposed 模块</p>

<p>
  <b>支持框架</b>：
  <b><a href="https://github.com/LSPosed/LSPosed">LSPosed</a></b> /
  <b><a href="https://github.com/LSPosed/LSPatch">LSPatch</a></b>
</p>
</div>

---

## 项目简介

- 此项目在前 HookVip 的基础上重构于 **2024.10.30**
- 这是一款基于 **Xposed API** 开发的 Xposed 模块
- 主要用于对部分 App：
  - 解锁部分会员功能与高级功能
  - 解除部分功能限制
  - 提供额外拓展功能
- 旨在优化用户使用体验，为用户提供更方便的功能入口与增强能力

---

## 功能分类

本模块当前功能主要分为以下 3 类：

| 功能类型 | 作用说明 | 启用方式 |
|---|---|---|
| 破解功能 | 用于解锁部分 App 的会员功能、高级功能或部分限制 | 勾选目标应用后直接生效 |
| 拓展功能 | 为目标应用提供额外增强功能，需要在模块内手动开启 | 在模块主页进入对应应用配置 |
| 拓展应用 | 将功能入口或功能开关注入到目标应用内部页面 | 在应用内找到注入开关后开启 |

### 1. 破解功能
适用于直接生效的功能。  
通常只需要在框架中勾选对应应用，重启后即可使用。

### 2. 拓展功能
适用于需要在模块内进行额外设置的功能。  
例如进入模块侧滑栏，找到对应应用后，再选择性开启你需要的功能。

### 3. 拓展应用
适用于将功能开关注入到目标应用设置页、用户页或相关页面的功能。  
需要先勾选应用并重启，再进入应用内找到对应开关后启用。

---

## 使用说明

### 破解功能

1. 在框架中勾选对应应用
2. 重启对应应用后生效
3. 如果没有生效，请尝试登录一下账号
4. 如果仍然不生效，可能是当前版本已失效或暂不兼容
5. 如遇到功能不生效或其他问题，请前往仓库 [Issues](https://github.com/Xposed-Modules-Repo/top.hookvip.pro/issues) 按模板提交反馈

---

### 拓展功能

1. 先前往模块主页
2. 点击左上角，或在主页右滑打开侧滑栏
3. 进入 **拓展功能** 页面
4. 找到并点击你需要作用的应用
5. 选择性开启你需要使用的功能
6. 确保总开关已开启
7. 重启对应应用后生效

---

### 拓展应用

1. 在框架中勾选对应应用
2. 重启该应用
3. 前往应用设置页 / 用户信息页 / 相关页面
4. 模块会注入对应的功能入口或功能开关
5. 找到并开启你需要使用的功能
6. 如有需要，重新启动应用后生效

---

## 框架限制

### LSPosed

- 可正常使用本模块全部功能
- 推荐优先使用该框架

### LSPatch

- 仅允许使用 **破解功能**
- 无法使用 **拓展应用** 功能
- 部分高风险破解功能也会被限制使用
- 不支持 **内置模式**
- 仅可使用 **本地模式**
- 当前不受理该框架环境下的兼容性反馈

---

## 问题反馈

当前仅接受 **[GitHub Issues](https://github.com/Xposed-Modules-Repo/top.hookvip.pro/issues)** 反馈，**不通过群消息处理问题**。

请根据问题类型选择对应模板：

- [问题反馈](https://github.com/Xposed-Modules-Repo/top.hookvip.pro/issues/new?template=ISSUE_TEMPLATE_BUG.yml)：功能不生效、Bug、异常情况
- [适配请求](https://github.com/Xposed-Modules-Repo/top.hookvip.pro/issues/new?template=ISSUE_TEMPLATE_SUPPORT_APP.yml)：新需求、建议、应用适配请求

---

## 免责声明

- 应用内所有功能仅供学习交流使用，请勿用于商业或违法用途
- 本模块完全免费使用，不存在收费盈利
- 如果你是付费购买的，请联系售卖者退款
- 禁止售卖、倒卖或二次打包分发本模块
- 因使用本模块产生的任何后果，由使用者自行承担
- 如有侵权问题，请联系邮箱：<hookvip@163.com>

---

## 赞助打赏

- 模块自 **2022.08.12** 起持续维护至今，适配、测试、排查与更新都需要投入不少时间与精力
- 如果这个模块确实帮到了你，或者替你省下了一些时间，欢迎自愿赞助支持
- 你的每一份支持，都会成为后续维护、版本适配与功能更新的动力
- 模块会继续保持免费发布，赞助仅作为对长期维护的支持

**补充说明：**

- 赞赏满 30 元可加入模块专属内测群
- 请联系 TG：[`@lovejiuwu`](https://t.me/lovejiuwu)
- 联系前请先阅读 [频道置顶消息](https://t.me/HookVipCl/)

<img width="200" height="200" alt="赞助码" src="https://github.com/user-attachments/assets/4d2143e7-6a06-44ac-9e55-a2810585561f" />
