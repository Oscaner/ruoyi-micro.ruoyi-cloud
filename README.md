## 平台简介

若依是一套全部开源的快速开发平台，毫无保留给个人及企业免费使用。

官方链接: https://gitee.com/y_project/RuoYi-Cloud

## Devops

基于 Ansible 实现的 Devops 部署脚本，便于 RuoYi 快速启动。

### Prepare

- docker
- ansible
- docker-compose (optional)
- k8s (optional)

### How to use it?

1. Create file `devops/vars/main.local.yml`

```md
---
docker_username: xxx
docker_password: xxx
docker_registry_url: https://index.docker.io/v1/

maven_local_repo_dir: xxx
```

2. Run ansible

```sh
> cd devops
> ansible-playbook playbook.yml [--extra-vars "maven_jar_version=v1.0.1"]
```

> WIP
