# :rocket: Task-3

## 1. Background

### i. Docker

**容器** 代表一个打包好的软件运行环境。**容器镜像** 是一系列静态文件。**容器运行时** 可运行镜像来生成容器。广义上的 Docker 可以表示运行的 Docker container，可以表示静态的 Docker image，可以表示运行 container 的 Docker Engine，也可以表示一个帮助开发者开发、运行、发布应用的平台。

通过 [这里](https://docs.docker.com/engine/install/) 安装 Docker。

Dockerfile 用于定制镜像，可通过 [这里](https://docs.docker.com/develop/develop-images/dockerfile_best-practices/) 学习 Dockerfile。如果你认为这不够仔细，可以阅读 [Dockerfile Reference](https://docs.docker.com/engine/reference/builder/)。

### ii. docker-compose

现在可以直接使用 docker compose 来代替 docker-compose，详见 [此处](https://docs.docker.com/compose/#compose-v2-and-the-new-docker-compose-command)。

docker-compose.yml 用于告知 docker compose 如何运行。由于 compose 可 build 与 run，因此 docker-compose.yml 有两个重要的 `element`：[docker-compose file build](https://docs.docker.com/compose/compose-file/build/) & [docker-compose file deploy](https://docs.docker.com/compose/compose-file/deploy/)。

docker-compose 还有其余 `element`，可见 [docker-compose file specification](https://docs.docker.com/compose/compose-file/)。

### iii. GitHub Actions

常用于 [CI/CD](https://about.gitlab.com/topics/ci-cd/)。

使用 .github/workflows 下的 *.yaml 文件来定义 GitHub Actions 的 workflow。可通过 [这里](https://docs.github.com/en/actions/using-workflows/about-workflows) 从无到有触发有用的 workflow。（不过 GitHub 的 documentation 无一不抽象）

## 2. Tasks

* **Docker** | [tongji-undergrad-thesis-env](https://github.com/TJ-CSCCG/tongji-undergrad-thesis-env)：

  * 进一步缩小镜像体积；
  * 更好地利用缓存层加速本地构建。

* **GitHub Actions** | [tongji-undergrad-thesis-env](https://github.com/TJ-CSCCG/tongji-undergrad-thesis-env)：

  目前使用 [release workflow](https://github.com/TJ-CSCCG/tongji-undergrad-thesis-env/actions/workflows/release.yaml) 发布镜像到 hub.docker.com 上，使用 [test workflow](https://github.com/TJ-CSCCG/tongji-undergrad-thesis-env/actions/workflows/test.yaml) 测试镜像是否可以正常构建。但并没有测试可否正常编译 [tongji-undergrad-thesis](https://github.com/TJ-CSCCG/tongji-undergrad-thesis)。

  * 在 test workflow 中测试镜像是否可用于编译模板。

* **GitHub Actions** | [tongji-undergrad-thesis](https://github.com/TJ-CSCCG/tongji-undergrad-thesis)：

  * 使用 BasicTeX，而非使用 install-tl 从零安装。
