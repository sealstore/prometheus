# 使用方法
注意，请使用sealos最新版本，如果是老版本sealos安装的集群不会自动生成sealos配置文件，需要自己手动配置，会输出日志教你如何配置

本地拉取(先到[release页面](https://github.com/sealstore/prometheus/releases)下载好tar包到本地)：
```
wget https://github.com/sealstore/prometheus/releases/download/v0.31.1/prometheus.tar
sealos install --pkg-url prometheus.tar
```
或者远程拉取：
```
sealos install --pkg-url https://github.com/sealstore/prometheus/releases/download/v0.31.1/prometheus.tar
```

# 访问方式
grafana http://集群节点IP:30000 初始账户密码 admin/admin

# 为什么要用此包
1. tar包中包含yaml文件，镜像文件，离线无忧
2. 即便你没有镜像仓库，sealos也会帮你把镜像导入到集群节点上
3. 一键安装省心
4. 实现上使用高大上的prometheus operator,各组件实现高可用
