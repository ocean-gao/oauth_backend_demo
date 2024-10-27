
# 用 Go 简单实现 Github 授权登录并获取 github 用户信息

## 1. 相关链接

- [用 Go 简单实现 Github 授权登录并获取 github 用户信息](https://juejin.cn/post/7414732978141544463)
- [没错，用三方 Github 做授权登录就是这么简单！（OAuth2.0 实战）](https://cloud.tencent.com/developer/article/1663102)
- [一口气说出 OAuth2.0 的四种授权方式](https://mp.weixin.qq.com/s?__biz=MzAxNTM4NzAyNg==&mid=2247487003&idx=1&sn=47cd6b064a7fc3b3df8f6f4c3f7669a7)
- [理解 OAuth 2.0 - 阮一峰](https://www.ruanyifeng.com/blog/2014/05/oauth_2_0.html)
- [Github 文档 - 授权 OAuth 应用](https://docs.github.com/zh/apps/oauth-apps/building-oauth-apps/authorizing-oauth-apps)

## 2. 运行

> 注：`main.go` 文件中先填写 Github Oauth 应用的 相关信息。

```go
go run main.go
```

浏览器访问 `http://localhost:8080`，重定向到 `http://localhost:8080/api/auth?code=4e20e708e9178f5ef885`，响应内容如：

```
{ocean_gao https://avatars.githubusercontent.com/u/73287541?v=4 gho_VWQ7*****oZyIA}
```