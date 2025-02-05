### 1.官方镜像路径前面加域名
```shell
docker pull docker.example.com/stilleshan/frpc:latest
```
```shell
docker pull docker.example.com/library/nginx:stable-alpine3.19-perl
```

### 2.一键设置镜像加速
修改文件 `/etc/docker/daemon.json`（如果不存在则创建）
```shell
sudo mkdir -p /etc/docker
sudo tee /etc/docker/daemon.json <<-'EOF'
{
  "registry-mirrors": ["https://docker.example.com"]  # 请替换为您自己的Worker自定义域名
}
EOF
sudo systemctl daemon-reload
sudo systemctl restart docker
```
# 🛠️ 第三方 DockerHub 镜像服务

**注意:**
- 以下内容仅做镜像服务的整理与搜集，未做任何安全性检测和验证。
- 使用前请自行斟酌，并根据实际需求进行必要的安全审查。
- 本列表中的任何服务都不做任何形式的安全承诺或保证。

| DockerHub 镜像仓库 | 镜像加地址 |
| ------------------ | ----------- |
| [bestcfipas镜像服务](https://t.me/bestcfipas/1900) | `https://docker.registry.cyou` |
|  | `https://docker-cf.registry.cyou` |
| [zero_free镜像服务](https://t.me/zero_free/80) | `https://docker.jsdelivr.fyi` |
|  | `https://dockercf.jsdelivr.fyi` |
|  | `https://dockertest.jsdelivr.fyi` |
| [docker proxy](https://dockerpull.com/) | `https://dockerpull.com` |
| [docker proxy](https://dockerproxy.cn/) | `https://dockerproxy.cn` |
| [Docker镜像加速站](https://hub.uuuadc.top/) | `https://hub.uuuadc.top` |
|  | `https://docker.1panel.live` |
|  | `https://hub.rat.dev` |
| [DockerHub 镜像加速代理](https://docker.anyhub.us.kg/) | `https://docker.anyhub.us.kg` |
|  | `https://docker.chenby.cn` |
|  | `https://dockerhub.jobcher.com` |
| [镜像使用说明](https://dockerhub.icu/) | `https://dockerhub.icu` |
| [Docker镜像加速站](https://docker.ckyl.me/) | `https://docker.ckyl.me` |
| [镜像使用说明](https://docker.awsl9527.cn/) | `https://docker.awsl9527.cn` |
| [镜像使用说明](https://docker.hpcloud.cloud/) | `https://docker.hpcloud.cloud` |
| [DaoCloud 镜像站](https://github.com/DaoCloud/public-image-mirror) | `https://docker.m.daocloud.io` |
| [AtomHub 可信镜像仓库平台](https://atomhub.openatom.cn/) (只包含基础镜像，共336个) | `https://atomhub.openatom.cn` |

# 🙏 鸣谢

[muzihuaner](https://github.com/muzihuaner)、[V2ex网友](https://global.v2ex.com/t/1007922)、[ciiiii](https://github.com/ciiiii/cloudflare-docker-proxy)、[ChatGPT](https://chatgpt.com/)、[白嫖哥](https://t.me/bestcfipas/1900)、[zero_free频道](https://t.me/zero_free/80)、[dongyubin](https://github.com/cmliu/CF-Workers-docker.io/issues/8)、[kiko923](https://github.com/cmliu/CF-Workers-docker.io/issues/5)
