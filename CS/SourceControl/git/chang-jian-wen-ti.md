# 常见问题

遇到以下问题，尝试关闭代理。如果有自己使用的代理，重新设置，注意端口号

## 1. 代理问题 <a href="#articlecontentid" id="articlecontentid"></a>

以下问题因为网络原因导致，请检查代理

> 1. LibreSSL SSL\_connect: SSL\_ERROR\_SYSCALL in connection to github.com:443
> 2. fatal: unable to access : Empty reply from server

```sh
// 设置代理shell
git config --global http.proxy "http://localhost:1080"
git config --global https.proxy "http://localhost:1080"

// 取消代理
git config --global --unset http.proxy
git config --global --unset https.proxy
git config --global --unset socks.proxy

// 查看git设置，检查代理是否设置成功
git config -l
```
