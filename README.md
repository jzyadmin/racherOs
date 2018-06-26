# [racherOs官方文档地址](https://rancher.com/docs/os/v1.x/en/quick-start-guide/)
系统默认docker加载组件

#### 查看系统docker

> sudo system-docker ps


#### 查看配置信息
> 系统中查看配置信息 sudo ros config get 

> 系统中修改配置信息 sudo ros config set 

> 系统中服务相关信息 sudo ros service


#### 设置dns信息
```
# 设置dns信息
sudo ros config set rancher.network.dns.nameservers"['192.168.1.1','0.0.0.0','8.8.8.8','8.8.4.4']"

# 写入设置信息
sudo ros config validate -i /var/lib/rancher/conf/cloud-config.yml

# 重启网络docker
sudo system-docker restart network

```

[查看更多内容](https://rancher.com/docs/os/v1.x/en/quick-start-guide/)
