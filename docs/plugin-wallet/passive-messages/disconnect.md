---
title: 断开连接网站消息
layout: docs
category: plugin
parent: plugin-wallet/passive-messages
---

消息标识： `disconnect`

**简介**

开发者可以监听此消息来获取网络的改变。

以下情况会产生此消息：

  1. DApp 请求连接，用户在弹窗中拒绝连接后

  2. 用户主动断开连接网站

**技术规范**

**代码示例**

Copy

    window.addEventListener('message', function (e) {
      if (e.data.message && e.data.message.action == "disconnect") {
          // handler logic
          console.log('got connect event', e.data)
      }
    })

[Previous连接网站成功消息](https://docs-zh.tronlink.org/cha-jian-qian-bao/bei-dong-jie-shou-tronlink-cha-jian-de-xiao-xi/lian-jie-wang-zhan-cheng-gong-xiao-xi)[Next即将废弃的消息](https://docs-zh.tronlink.org/cha-jian-qian-bao/bei-dong-jie-shou-tronlink-cha-jian-de-xiao-xi/ji-jiang-fei-qi-de-xiao-xi)

Last updated 2 years ago