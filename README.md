# Ansible 
远程执行脚本的自动化运维工具,使用ssh协议，主控机与客户机无需安装任何软件

默认执行 
1. 关闭selinux
2. 配置ssh登录
3. 配置阿里云yum源并安装 wget|telnet|lrzsz|vim|git|curl|tree
4. 安装docker docker-ce-20.10.3-3.el7
5. 初始化docker-swarm集群 

## 版本
2.9.1

## install ansible
centos 
`yum install ansible`
other [ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)

## ssh
ssh-keygen -t rsa

## clone
`
cd etc && git clone
`
## change ip
node 节点为受控全部节点

worker 为swarm worker节点

manager 为swarm manager节点


## start
`
ansible-playbook playbook.yml
`

