# wechat-send-action

通过微信测试号向用户发送模板消息

# Usage

```bash
- uses: xiaoxuan6/github@main
  with:
    wechat_user: ${{ secrets.WECHAT_USER }}
    wechat_appid: ${{ secrets.WECHAT_APPID }}
    wechat_appsecret: ${{ secrets.WECHAT_APPSECRET }}
    wechat_templateid: ${{ secrets.WECHAT_TEMPLATEID }}
    message: "test"
    url: "www.baidu.com"
```

