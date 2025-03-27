# Vultr 云服务器购买与配置额外 IPv4 地址完整指南

Vultr 云服务平台支持为 VPS 实例购买额外的 IPv4 地址，无论是为 IPv6 Only 方案添加 IPv4 支持，还是为常规方案扩展 IP 资源，本教程将详细介绍完整的操作流程。购买完成后，我们还需要进行相应的网络配置才能使新增的 IP 地址生效。

## 一、Vultr 额外 IPv4 地址购买流程

1. 登录 [Vultr 官网](https://bit.ly/VuLtr)后台
2. 进入目标实例的 "Settings" 页面
3. 点击 "Add Another IPv4 Address" 选项
4. 确认费用信息（$0.003/小时）
5. 点击 "Add IPv4 Address" 完成购买

购买成功后，在 "Settings" 页面可以看到新增的 IPv4 地址（Additional IP）与主 IP（Main IP）并列显示。

👉 [【点击查看】2025年最新 Vultr 优惠码及特价云服务器方案汇总](https://bit.ly/VuLtr)

## 二、不同 Linux 系统的 IPv4 配置方法

### CentOS 系统配置

#### CentOS 6/7 配置步骤
1. 修改 `/etc/sysconfig/network-scripts/ifcfg-eth0`：
bash
DEVICE=eth0
ONBOOT=yes
BOOTPROTO=static
IPADDR=主IP地址
NETMASK=子网掩码
GATEWAY=网关地址
DNS1=108.61.10.10

2. 创建 `/etc/sysconfig/network-scripts/ifcfg-eth0:1`：
bash
DEVICE=eth0:1
BOOTPROTO=static
IPADDR=额外IP地址
NETMASK=255.255.255.255
ONBOOT=yes

3. 重启网络服务：
bash
service network restart

#### CentOS 8 配置方法
修改 `/etc/sysconfig/network-scripts/ifcfg-ens3`：
bash
TYPE="Ethernet"
DEVICE="ens3"
ONBOOT="yes"
BOOTPROTO="none"
IPADDR=主IP地址
PREFIX=子网前缀
GATEWAY=网关地址
DNS1=108.61.10.10
IPADDR1=额外IP地址
PREFIX1=32

### Debian/Ubuntu 系统配置

#### Debian 9/10 & Ubuntu 16.04+ 配置
修改 `/etc/network/interfaces`：
bash
auto ens3
iface ens3 inet static
    address 主IP地址
    netmask 子网掩码
    gateway 网关地址
    dns-nameservers 108.61.10.10

auto ens3:1
iface ens3:1 inet static
    address 额外IP地址
    netmask 255.255.255.255

#### Ubuntu 17.10+ 配置
修改 `/etc/netplan/10-ens3.yaml`：
yaml
network:
  version: 2
  ethernets:
    ens3:
      dhcp4: no
      addresses: [主IP地址/子网前缀,额外IP地址/32]
      gateway4: 网关地址
      nameservers:
        addresses: [108.61.10.10]

## 三、配置验证与实例重启

完成上述配置后，建议执行以下操作：

1. 使用 `ip a` 命令检查新 IP 是否已生效
2. 在 Vultr 控制面板重启实例
3. 测试新 IP 的网络连通性

通过以上步骤，您已成功为 Vultr 云服务器添加并配置了额外的 IPv4 地址。如需更多 Vultr 使用技巧，可以参考官方文档或相关技术社区。