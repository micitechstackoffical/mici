# 添加文档教程

## 问题 

### Github提交时网络无法连接
```
fatal: unable to access 'https://github.com/micitechstack/mici.git/': OpenSSL SSL_read: Connection was reset, errno 10054
```
解决办法1:
尝试取消git的代理
```
git config --global http.sslVerify "false"
git config --global --unset http.proxy
git config --global --unset https.proxy
```