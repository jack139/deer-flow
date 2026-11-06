# TEST

```bash
# 拉取 sandbox 镜像（首次运行或镜像更新时执行）
make docker-init

# 启动服务（会根据 config.yaml 自动判断 sandbox 模式）
make docker-start

# 使用国内源
# APT_MIRROR="mirrors.aliyun.com"
# UV_INDEX_URL="https://mirrors.aliyun.com/pypi/simple/"
# NPM_REGISTRY="https://registry.npmmirror.com"
APT_MIRROR="mirrors.aliyun.com" \
    NPM_REGISTRY="https://registry.npmmirror.com" \
    UV_INDEX_URL="https://mirrors.aliyun.com/pypi/simple/" \
    make docker-start
```