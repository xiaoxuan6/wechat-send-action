# wechat-send-action

通过微信测试号向用户发送模板消息

# Wechat configuration

[微信测试号](https://mp.weixin.qq.com/debug/cgi-bin/sandbox?t=sandbox/login)

扫码登录成功后创建模板消息，例如：

|序号|模板ID(用于接口调用)|模板标题|模板内容|
|:---|:---|:---|:---|
|1|xxx|消息通知|内容：{{content.DATA}}|

# Usage

```bash
- uses: xiaoxuan6/wechat-send-action@main
  with:
    wechat_user: ${{ secrets.WECHAT_USER }}
    wechat_appid: ${{ secrets.WECHAT_APPID }}
    wechat_appsecret: ${{ secrets.WECHAT_APPSECRET }}
    wechat_templateid: ${{ secrets.WECHAT_TEMPLATEID }}
    message: "test"
    url: "www.baidu.com"
```

