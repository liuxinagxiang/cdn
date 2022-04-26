### CentOs-6-Vault.repo

jsdelivr-cdn
```
github:
https://cdn.jsdelivr.net/gh/user/repo@version/file
https://cdn.jsdelivr.net/gh/liuxinagxiang/cdn/CentOs-6-Vault/CentOs-6-Vault-Aliyun.repo

npm:
https://cdn.jsdelivr.net/npm/package@version/file
```
statically-cdn
```
github:
https://cdn.staticaly.com/gh/:user/:repo/:tag/:file
https://cdn.staticaly.com/gh/liuxinagxiang/cdn/master/CentOs-6-Vault/CentOs-6-Vault-Aliyun.repo

gitlab:
https://cdn.statically.io/gl/:user/:repo/:tag/:file
```

how to use:
```
#备份
mv -v /etc/yum.repos.d/CentOS-Base.repo{,-backup}
#替换为官方Vault源
wget -O /etc/yum.repos.d/CentOS-Base.repo https://cdn.jsdelivr.net/gh/liuxinagxiang/cdn/CentOs-6-Vault/CentOs-6-Vault-Official.repo
#替换为阿里云Vault镜像
curl -o /etc/yum.repos.d/CentOS-Base.repo https://cdn.jsdelivr.net/gh/liuxinagxiang/cdn/CentOs-6-Vault/CentOs-6-Vault-Aliyun.repo
```
